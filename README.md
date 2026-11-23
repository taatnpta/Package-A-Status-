# TA2028 · Package A Document Status

Dashboard ติดตามสถานะเอกสาร Package A (01 Plot Plan, 02 Summary Worklist, 03 Drawing, 04 Job Card Checklist, 05 Blind List) ทั้ง 13 Area
ใช้ Supabase เป็นฐานข้อมูล บันทึกออนไลน์ และทุกคนเห็นข้อมูลแบบ Real-time

## วิธีเปิด
- เปิดไฟล์ `index.html` ในเบราว์เซอร์ หรือ
- เปิดผ่าน GitHub Pages (Settings → Pages → Branch: `main` / root)

## ตั้งค่า Supabase
1. รัน SQL สร้างตาราง `pkga_items` และ `pkga_log` ใน Supabase SQL Editor
2. ใส่ Supabase URL และ publishable/anon key ในโปรแกรม (ปุ่ม ⚙ หรือแก้ค่าในส่วนต้นของ script)

## หน้าในโปรแกรม
- **Overview:** Overall Status ทั้ง 13 Area และ Dashboard ราย Area
- **Detail by EQ Tag:** ดูและแก้สถานะราย Equipment
- **Log · Import / Export:** ลากไฟล์ Excel เพื่ออัปเดตข้อมูล, Export และดูประวัติการแก้ไข

> ⚠️ Repo นี้เป็น Public — ใครที่มีไฟล์นี้จะเข้าถึง Database ได้ตามสิทธิ์ที่ตั้งไว้ใน Supabase (RLS)
