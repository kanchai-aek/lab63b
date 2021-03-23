# การทดลองที่ 2 เรื่อง การเขียนโปรแกรมค้นหาไวไฟ

## วัตถุประสงศ์
1.เพื่อเข้าใจการต่อไมโครคอนโทรเลอร์เพื่อเชื่อมต่อกับคอมพิวเตอร์ ในการรันโปรแกรม
2.เพื่อเข้าใจในวิธีการรันโปรแกรมลงบนไมโครคอนโทรเลอร์
3.เพื่อศึกษาการทำงานของโปรแกรมค้นหาไวไฟ
## อุปกรณ์ในการทดลอง
1.ไมโครคอนโทรเลอร์ ESP01
2.อุปกรณ์ต่อ USB
3.ซีเรียลพอร์ต
4.คอมพิวเตอร์
## ศึกษาข้อมูลเบื้องต้น
การทดลอง https://www.youtube.com/watch?v=yBjab0UNuB8
การเขียนเนื้อหาใน Repository
Mastering Markdown https://guides.github.com/features/mastering-markdown/

MARKDOWN SYNTAX https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

Basic writing and formatting syntax https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax

GitHub Flavored Markdown Spec https://github.github.com/gfm/

มาสร้าง Web Hosting ใช้กันฟรีๆกับ Github.io กันเถอะ https://sirawit0676.medium.com/มาสร้าง-web-hosting-ใช้กันฟรีๆกับ-github-io-กันเถอะ-d527e8c3bb9b

ทำเว็บเพจง่ายมากเว่อร์ https://medium.com/pranworks/ทำเว็บเพจง่ายมากเว่อร์-githubpages-e823313d06dc

วิธีการ Deploy เว็บไซต์แบบฟรีๆ ด้วย Github Pages https://devahoy.com/blog/2017/02/how-to-host-website-on-github-pages/
## วิธีทำรทดลอง
1.เขียนโปรแกรม (ซอสโค้ด)
2.เปิดซอสโค้ด![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823939317978103838/unknown.png)![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823939396830494760/unknown.png)
3.รันโปรแกรมลงบนไมโครคอนโทรเลอร์ โดยพิมพ์  pio run -t upload ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823939571627589683/unknown.png)
4.ในขณะรันกดปุ่มสีดำที่ไมโครคอนโทรเลอร์แร้วกดปุ่ม Reset ไฟสีฟ้าจะกระพิบ
5.พิมพ์ pio device monitor เพื่อดูผลการรัน ![alt text](https://media.discordapp.net/attachments/337849529179308033/823939890764185610/unknown.png?width=1191&height=670)
## บันทึกผลการทดลอง
  จาการทดลอง เมื่อพิมพ์ pio device monitor ผลลัพธ์จาการรันจะแสดงบนหน้าจอ คือ ไมโครคอนโทรเลอร์จะสแกนหาไวไฟ โดยจำนวนตัวของสัญญาณไวไฟขึ้นยุกับจำนวนความแรงของสัญญาณที่ได้รับ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823940068066328639/unknown.png)
เมื่อกดปุ่ม Reset ไมโครคอนโทรเลอร์ก็จะเริ่มสแกนหาไวไฟใหม่ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823940255005802516/unknown.png)
## อภิปรายผลการทดลอง
  จากการทดลองเมื่อกดรันโปรแกรมจะแสดงผลลัพธ์ออกทางหน้าจอ  คือ มโครคอนโทรเลอร์จะสแกนหาไวไฟ โดยจำนวนตัวของสัญญาณไวไฟขึ้นยุกับจำนวนความแรงของสัญญาณที่ได้รับ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823940068066328639/unknown.png)
  เมื่อกดปุ่ม Reset ไมโครคอนโทรเลอร์ก็จะเริ่มสแกนหาไวไฟใหม่ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823940255005802516/unknown.png)
## คำถาม
1. การ Upload Program ต้องกด port ชนิดใด

![alt text](https://media.discordapp.net/attachments/337849529179308033/823949173123842068/unknown.png)

ตอบ Port 0
