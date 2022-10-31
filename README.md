# atom-package-template

## วิธีสร้าง Package ขึ้นไปบน atom.io

0. ดาวน์โหลด [atom](https://atom.io) ก่อน 
1. สมัครสมาชิก atom.io ด้วยการ connect กับ github
2. ไปที่ [account](https://atom.io/account) เพื่อคัดลอก API Token
3. สร้าง Repositories ใหม่ ที่ github.com ให้ branch เริ่มต้นเป็น master ไม่ใช่ main
4. ใช้ 2 ไฟล์ในโปรเจคนี้ คือ README.md และ package.json
5. แก้ไข package.json ตรง name, theme, description, keywords
6. แก้ไข README.md ตามใจชอบ
7. commit จากนั้นก็ push ขึ้น github
8. พิมพ์ command `apm publish minor` หรือ `apm publish patch`
9. ครั้งแรกมันจะถามหา token ให้ใส่ token ในขั้นตอนที่ 2
10. หากเกิด error ให้ลองไปดู https://atom.io/users/{username-ของคุณ}  ก่อนว่า package ขึ้นไปหรือยัง เพราะมันอาจขึ้นไปแล้ว

## การอัพเดตเวอร์ชัน
1. แก้ไข README.md หรือ package.json
2. commit จากนั้นก็ push ขึ้น github
3. พิมพ์ command `apm unpublish`
4. ตอบ yes
5. พิมพ์ command `apm publish patch` หรือ `apm publish minor`
6. หากขึ้นตัวแดง ให้ไปเช็คที่ลิ้งค์ของ package ก่อน เพราะบางทีมันก็อัพเดตไปแล้ว