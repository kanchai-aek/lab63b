#การทดลองที่3

##วัตถุประสงค์
1.เพื่อศึกษาการใช้โปรแกรมเอ้าพุทสัญญาณดิจิทัลบนmicrocontroller

##อุปกรณ์การทดลอง
1.microcontroller ESP-01
2.USB serial port
3.Adepterโดย port 0ต่อกับเส้นสีขาว

##ศึกษาข้อมูลเบื้องต้น
1.https://www.youtube.com/watch?v=CCnN1WJsXQY

##วิธีการทำการทดลอง
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923037723426836/unknown.png)
1.เสียบAdepterเข้ากับUSB serial port
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923153708908584/unknown.png)
2เสียบmicrocontroller ESP-01เข้ากับAdepter
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923252144504842/unknown.png)
3เนื้อหาโปรแกรมคือ port 0 เป็นoutputและวนลูปตลอดโดยทุก500 millisecแล้วนับเลขขึ้นไปเรื่อยๆ โดยถ้าเป็นเลขคี่ให้ on แต่ถ้าเป็นเลขคู่ให้off
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923353546522673/unknown.png)
4พิมpio run -t upload
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923483230732298/unknown.png)
5พอโปรแกรมuploadเสร็จก็พิม pio device monitor

##การบันทึกผลการทดลอง
ตอนonไฟสีเขียวจะสว่างและไฟสีฟ้าจะดับ
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823925611500011570/unknown.png)
ตอนoffไฟสีฟ้าจะสว่างและไฟสีเขียวจะดับ
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823924908979126292/unknown.png)
##อภิปรายผลการทดลอง
จากการทดลองพบว่าทุกๆครึ่งวินาทีโปรแกรมจะแสดงเอ้าพุทออกมาเป็นonสลับกับoffแล้วไปดูที่LEDที่ต่อกับAdepterก็จะพบว่าที่port 0 LEDสีเขียวก็จะเปล่งแสงออกมาตอนที่เป็นonและจะดับเมื่อตอนเป็นoff ส่วนสีน้ำเงินก็ทำงาสลับกับสีเขียวสลับแบบนี้ไปเรื่อยๆ
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823924908979126292/unknown.png)

##คำถามการทดลอง
1. เพราะเหตุใด LED ถึงสลับกันติด

![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823925611500011570/unknown.png)

คำตอบ เพราะ Input เลขคี่เป็น on เลขคู่เป็น off ไฟจึงติดเฉพาะช่วงที่เป็น on 
