# ANSWER — นภัสกร ทิมินกุล 671540005027-1

- Platform: Render
- Production URL: https://ksu-coffee-671540005027-1-1.onrender.com

## คำตอบ

1. เลือก Render ซึ่งรัน Web Service ด้วย Container โดยใช้ `server.js` เป็นไฟล์เริ่มต้นผ่านคำสั่ง `node server.js`

2. ตั้งค่า `STUDENT_ID` ใน Environment Variables บน Render ห้าม commit `.env` เพราะอาจเปิดเผยข้อมูลสำคัญ หาก API แสดง `NOT SET` อาจเกิดจากไม่ได้ตั้งตัวแปร ตั้งชื่อผิด หรือยังไม่ได้ Deploy หลังแก้ไขค่า

3. ครั้งแรก 3.223900 วินาที / ครั้งที่สอง0.360866วินาที — เวลาตอบสนองอาจแตกต่างกัน เพราะ Render Free อาจพักบริการเมื่อไม่มีการใช้งาน ทำให้คำขอแรกใช้เวลาเริ่มระบบนานกว่า

4. เมื่อ `git push` ระบบ Render จะตรวจพบ commit ใหม่และ Deploy อัตโนมัติ หลัง Deploy เสร็จหน้าเว็บแสดง `Menu v2` และค่า `commit` ใน `/api/info` ต้องตรงกับ `git log -1 --format=%H`

5. ไม่สามารถนำ Docker Compose ที่มี 2 services ไป Deploy ตรง ๆ บน Web Service ที่เลือกได้ เพราะต้องตั้งค่าการรันบริการและเครือข่ายให้ตรงกับรูปแบบที่แพลตฟอร์มรองรับ