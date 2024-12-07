ฝากถึงอาจารย์นะครับวิชา IT410


วิธีการรันโปรเจค
โหลดไฟล์แบบ zip
1.ในไฟล์โปรเจคจะมีไฟล์ MySQL 1 อันชื่อ book_management_book.sql แล้วนำไป import MySQL Workbeach 8.0 CE 
2.สร้าง schema ชื่อ 'book_management' แล้ว import ไฟล์ที่ผมแปะไว้คือ book_management_book.sql
3.อย่าลืมเปลี่ยนรหัสผ่านที่ ไฟล์ backend --> server.js
const connectDB = async () => {
    try {
        db = await mysql.createConnection({
            host: 'localhost',
            user: 'root',
            password: '1234', <---- ตรงนี้ครับ เปลี่ยนเป็นรหัสของอาจารย์
            database: 'book_management'
4.วิธีการรัน เปิด terminal 2 อัน แล้วใส่โค้ดตามนี้ครับ
อันแรกคือ cd backend แล้่วใส่ nodemon server.js จะมีคำขึ้นว่า 
Connected to database!
Server running on port 3000
อันสองคือ ng serve
โปรเจคจะรันบน http://localhost:4200/
ขอบคุณครับ


version ที่ใช้ในการทำโปรเจค
Angular CLI: 16.2.16
Node: 18.20.5
Package Manager: npm 6.14.18
OS: win32 x64
