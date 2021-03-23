##การทดลองที่4

##วัตถุประสงค์
1.เพื่อศึกษาการใช้โปรแกรมอินพุทสัญญาณดิจิทัลบนmicrocontroller

##อุปกรณ์การทดลอง
1.microcontroller ESP-01
2.USB serial port
3.Adepterโดย port 0ต่อกับเส้นสีขาว และ port 2 ต่อกับเส้นสีเหลือง

##ศึกษาข้อมูลเบื้องต้น
1.https://www.youtube.com/watch?v=nFqoZT26U5k

##วิธีการทำการทดลอง
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923037723426836/unknown.png)
1.เสียบAdepterเข้ากับUSB serial port
![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823923153708908584/unknown.png)
2เสียบmicrocontroller ESP-01เข้ากับAdepter
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823928844356026368/unknown.png)
3เนื้อหาโปรแกรมคือ port 0 เป็นinputและport 2 เป็นoutputวนลูปตลอดโดยทุก100 millisecแล้วนับเลขขึ้นไปเรื่อยๆ โดยที่port0ถ้าเป็นเลขคี่ให้ on แต่ถ้าเป็นเลขคู่ให้off
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823931201785692200/unknown.png)
4.พิม pio run -t upload
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823931483945041940/unknown.png)
5.พอโปรแกรมuploadเสร็จก็พิม pio device monitor
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823932928538705981/unknown.png)
6.เอาเส้นสีขาวไปต่อเข้ากับเส้นสีดำดูว่าไฟติดไหม
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823933602685255730/unknown.png)
7.นำเซนเซอร์มาต่อกับAdeptor และนำสายสีขาวมาต่อด้วยตามภาพ

##การบันทึกผลการทดลอง
เมื่อเอาเส้นสีขาวไปจิ้มที่เส้นสีดำหลอดไฟจะติด (port 0 จิ้มไปที่ 0)
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823933141788917760/unknown.png)
เมื่อต่อเซนเซอร์เข้า ไฟจะติดเมื่อ อ่านค่าได้ 0 และไฟจะดับเมื่อไปบังแสงที่ตัวเซนเซอร์เพราะค่าจะอ่านออกมาเป็น 1
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823934106886078504/unknown.png)

##อภิปรายผลการทดลอง
การการทดลองพบว่าอินพุทของสัญญาณจะต้องเป็น0ไฟถึงจะติดและเมื่อนำตัวเซนเซอร์มาต่อกับAdepterก็จะพบว่าเมื่อเอามาบังเซนเซอร์ไฟLEDก็จะดับค่าที่อ่านออกมาก็คือ1และเมื่อเอามืออกไฟLEDก็จะติดค่าที่อ่านออกมาก็คือ0 ดังนั้น
1.ตอนไฟติด
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935515606777897/unknown.png)

2.ตอนไฟดับ
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935743961071656/unknown.png)

##คำถามการทดลอง
1. สัญญาณที่อยู่ตรงกลางคือสัญญาณจากอะไร

![alt text](https://media.discordapp.net/attachments/823924425152921641/823944654906458122/unknown.png?width=535&height=670)

คำตอบ สัญญาณจาก Sensored
