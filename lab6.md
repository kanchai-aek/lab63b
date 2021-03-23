## การทดลองที่ 6 เรื่อง การเขียนโปรแกรมสร้างไวไฟแอคเซสพอยต์ (Wifi AP)

# วัตถุประสงค์
1. เพื่อศึกษาการสร้างตัว WiFi AP
2. เพื่อศึกษาการ Coding ที่ไม่ต้องเชื่อมต่อกับ WiFi ที่มีอยู่
3. เพื่อศึกษาการ Run Sever ที่ไม่ต้องเชื่อมต่อกับ WiFi ที่มีอยู่

# อุปกรณ์ที่ใช้
1. ESP01
2. Micro USB
3. Computer
4. Phone

# ศึกษาข้อมูลเบื้องต้น
1. https://www.youtube.com/watch?v=T26DVHePlTs

# วิธีการทำการทดลอง
![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935196712927322/unknown.png)

1. เปืดการทดลองที่ 6 พร้อมกำหนดชื่อและรหัสผ่านของ WiFi

![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935565329203221/unknown.png)

2. ใส่ local ip, gateway และ subnet ของตัวMicrocontroller

![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935840170410004/unknown.png)

3. เปิด web sever ที่พอร์ต 80

![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823937015602085908/unknown.png)

4. สร้าง AP

![alt text](https://media.discordapp.net/attachments/823924425152921641/823937698028978206/unknown.png)

5. run program โดยการupload ลงบนmicrocontroller 

![alt text](https://media.discordapp.net/attachments/823924425152921641/823938261910028288/unknown.png)

6. Monitor ครั้งสุดท้ายเพื่อ reset

# การบันทึกผลการทดลอง

![alt text](https://media.discordapp.net/attachments/823924425152921641/823938539400986684/unknown.png)

ตรวจสอบว่ามี WiFi ที่สร้างขึ้นมาหรือไม่

# อภิปรายผลการทดลอง
  การทดลองที่ 6 เป็นการสร้าง Sever ที่ไม่มี WiFi อยู่จึงจำเป็นต้องสร้าง WiFi AP ขึ้นมาโดยสร้าง Code ลงบน Microcontroller แล้วให้
Microcontroller ทำการกระจายสัญญาณ

# คำถามหลังการทดลอง
1. หลังจากกำหนดชื่อและรหัสผ่านของ WiFi แล้วต้องทำขั้นตอนใดต่อ

![alt text](https://cdn.discordapp.com/attachments/823924425152921641/823935565329203221/unknown.png)

คำตอบ ใส่ local ip, gateway และ subnet ของตัวMicrocontroller
