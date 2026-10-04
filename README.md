# อรุณยนตรกิจ · AROON Auto Service

เว็บไซต์หน้าเดียวของอู่ซ่อมรถอรุณยนตรกิจ อ.สะเดา จ.สงขลา
เป็น HTML ล้วน ไม่ต้อง build ไม่ต้องติดตั้งอะไร

## โครงสร้าง

```
index.html      หน้าเว็บทั้งหมด (CSS + JS อยู่ในไฟล์นี้)
favicon.svg     ไอคอนแท็บเบราว์เซอร์
assets/         รูปหน้าร้าน, คลิปรีวิว, ภาพรีวิว Google
vercel.json     ตั้งค่า cache และ header บน Vercel
robots.txt      อนุญาตให้ Google เก็บข้อมูลหน้าเว็บ
```

## Deploy บน Vercel

1. Push repo นี้ขึ้น GitHub
2. ใน Vercel กด **Add New → Project** แล้วเลือก repo นี้
3. Framework Preset: **Other** · Build Command: เว้นว่าง · Output Directory: เว้นว่าง (หรือ `.`)
4. กด **Deploy**

## แก้ข้อมูลร้าน

ข้อมูลทั้งหมดอยู่ใน `index.html` ค้นหาแล้วแก้ได้เลย เช่น
- เบอร์โทร `081 599 5121` / `tel:0815995121`
- LINE `https://lin.ee/pWKsWKY`
- เวลาเปิด–ปิด: ข้อความในหน้า + สคริปต์ `shopStatus()` ท้ายไฟล์ + `openingHoursSpecification` ใน `<head>`
