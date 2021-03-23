# การทดลองที่ 1 การเขียนโปรแกรมเพื่อนบนไมโครคอนโทรเลอร์

## วัตถุประสงศ์
1.เพื่อเข้าใจการต่อไมโครคอนโทรเลอร์เพื่อเชื่อมต่อกับคอมพิวเตอร์ ในการรันโปรแกรม
2.เพื่อเข้าใจในวิธีการรันโปรแกรมลงบนไมโครคอนโทรเลอร์
## อุปกรณ์ในการทดลอง
1.ไมโครคอนโทรเลอร์ ESP01
2.อุปกรณ์ต่อ USB
3.ซีเรียลพอร์ต
4.คอมพิวเตอร์
## ศึกษาข้อมูลเบื้องต้น
การทดลอง https://www.youtube.com/watch?v=NLIUsWLEpmg
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
2.เปิดซอสโค้ด![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823930745214337045/unknown.png)![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823931658700324904/unknown.png)
3.รันโปรแกรมลงบนไมโครคอนโทรเลอร์ โดยพิมพ์  pio run -t upload ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823932385073561630/unknown.png)
4.ในขณะรันกดปุ่มสีดำที่ไมโครคอนโทรเลอร์แร้วกดปุ่ม Reset ไฟสีฟ้าจะกระพิบ
5.พิมพ์ pio device monitor เพื่อดูผลการรัน ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823932831926321172/unknown.png)
## บันทึกผลการทดลอง
  จาการทดลอง เมื่อพิมพ์ pio device monitor ผลลัพธ์จาการรันจะแสดงบนหน้าจอ คือ ตัวแปร Count จะนับเพิ่มขึ้นทีละ 1 ทุกๆ 1 วินาที ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823933124735008828/unknown.png)
เมื่อกดปุ่ม Reset ไมโครคอนโทรเลอร์ก็จะเริ่มนับใหม่ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823933280809517069/unknown.png)
## อภิปรายผลการทดลอง
  จากการทดลองเมื่อกดรันโปรแกรมจะแสดงผลลัพธ์ออกทางหน้าจอ  คือ ตัวแปร Count จะนับเพิ่มขึ้นทีละ 1 ทุกๆ 1 วินาที ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823933124735008828/unknown.png)
  เมื่อกดปุ่ม Reset ไมโครคอนโทรเลอร์ก็จะเริ่มนับใหม่ ![alt text](https://cdn.discordapp.com/attachments/337849529179308033/823933280809517069/unknown.png)
## คำถาม
1. การทดลองนี้มี delay เท่ากับเท่าไร

![alt text](https://media.discordapp.net/attachments/337849529179308033/823948515096657960/unknown.png)

ตอบ 1000 ms


