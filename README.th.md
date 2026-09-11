# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## ดาวน์โหลด

ลิงก์ด้านล่างชี้ไปที่แพ็กเกจเวอร์ชันล่าสุดเสมอ (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> การดาวน์โหลดทั้งหมดผ่าน `releases/latest/download/` ดังนั้นคุณจะได้รับแพ็กเกจล่าสุดเสมอโดยไม่ต้องอัปเดตที่อยู่นี้

## การแปลภาษา (Localization)

เราขอเชิญชวนทุกท่านร่วมมีส่วนร่วมในการแปลภาษาของโปรเจกต์นี้ ไม่ว่าจะเป็นการเพิ่มภาษาใหม่หรือปรับปรุงคำแปลที่มีอยู่ เรายินดีรับความช่วยเหลือทุกอย่าง

ข้อความที่แปลได้ทั้งหมดอยู่ในไดเรกทอรี `res/` แต่ละภาษามีโฟลเดอร์ของตัวเองตั้งชื่อตาม locale:

- `res/values/` — ข้อความเริ่มต้น/พื้นฐาน (จีนตัวย่อ) ใช้เป็นแหล่งอ้างอิง
- `res/values-en/` — อังกฤษ
- `res/values-ja/` — ญี่ปุ่น
- `res/values-ko/` — เกาหลี
- `res/values-ru/` — รัสเซีย
- `res/values-de/` — เยอรมัน
- `res/values-fr/` — ฝรั่งเศส
- `res/values-es/` — สเปน
- `res/values-pt/` — โปรตุเกส
- `res/values-it/` — อิตาลี
- `res/values-tr/` — ตุรกี
- `res/values-ar/` — อาหรับ
- `res/values-th/` — ไทย
- `res/values-vi/` — เวียดนาม
- `res/values-in/` — อินโดนีเซีย
- `res/values-ms/` — มาเลย์
- `res/values-zh-rTW/` — จีนตัวเต็ม

แต่ละโฟลเดอร์มีไฟล์ `strings.xml` แอตทริบิวต์ `name` ของแต่ละรายการ `<string>` คือคีย์และ**ห้ามแก้ไข** — ให้แปลเฉพาะข้อความระหว่างแท็กเท่านั้น

### วิธีแปล

1. Fork ที่เก็บนี้และโคลนลงในเครื่องของคุณ
2. เปิดไดเรกทอรี `res/` และค้นหาโฟลเดอร์ภาษาที่คุณต้องการทำงานด้วย
   - หากต้องการ**ปรับปรุงภาษาที่มีอยู่** ให้แก้ไข `strings.xml` ของภาษานั้นโดยตรง
   - หากต้องการ**เพิ่มภาษาใหม่** ให้คัดลอก `res/values-en/strings.xml` ไปยังโฟลเดอร์ใหม่ชื่อ `values-<locale>` (เช่น `values-nl` สำหรับภาษาดัตช์) แล้วแปลเนื้อหา
3. แปลค่าของแต่ละรายการ `<string>` ให้ใช้ `res/values/strings.xml` เป็นข้อมูลอ้างอิงสำหรับความหมายต้นฉบับเสมอ
4. รักษาตัวแทนที่ (เช่น `%1$s`, `%d`) และแท็กการจัดรูปแบบ (เช่น `<b>`, `\n`) ให้คงเดิมทุกประการ — ห้ามแปลหรือลบออกเด็ดขาด
5. ลบรายการที่มี `translatable="false"` หรือปล่อยไว้โดยไม่แตะต้อง เพราะไม่ควรแปล
6. ทดสอบการเปลี่ยนแปลงของคุณ จากนั้นเปิด Pull Request พร้อมระบุว่าคุณอัปเดตภาษาใด

ตัวอย่าง:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

ขอบคุณที่ช่วยทำให้ okmore เข้าถึงผู้คนทั่วโลกได้มากขึ้น!
