# คู่มือการตั้งค่าแอปใน Google Play Console

## 📱 ข้อมูลแอป
- **ชื่อแอป**: จดความดัน&น้ำตาล
- **Package Name**: com.myhealthtracker.app
- **Version**: 1.0.0
- **Version Code**: 1

## 🚀 ขั้นตอนการสร้างแอปใน Google Play Console

### 1. สร้างแอปใหม่
1. ไปที่ https://play.google.com/console
2. คลิก **"Create app"**
3. กรอกข้อมูล:
   - **App name**: จดความดัน&น้ำตาล
   - **Default language**: Thai (ไทย)
   - **App or game**: App
   - **Free or paid**: Free
   - **Declarations**: ✅ ตรวจสอบข้อตกลง
4. คลิก **"Create app"**

### 2. ตั้งค่าแอปพื้นฐาน
1. ไปที่ **"App content"**
2. กรอกข้อมูล:
   - **App category**: Medical
   - **Content rating**: 3+ (สำหรับทุกวัย)
   - **Target audience**: Adults 18+

### 3. ข้อมูลแอป (App details)
1. ไปที่ **"Main listing"**
2. กรอกข้อมูล:

**App name**: จดความดัน&น้ำตาล

**Short description** (80 ตัวอักษร):
```
แอปติดตามข้อมูลสุขภาพส่วนตัว
```

**Full description** (4000 ตัวอักษร):
```
จดความดัน&น้ำตาล เป็นแอปพลิเคชันสำหรับติดตามข้อมูลสุขภาพส่วนตัว 
สามารถบันทึกข้อมูลความดันโลหิต น้ำตาลในเลือด และชีพจร 
พร้อมแสดงกราฟและสถิติเพื่อติดตามสุขภาพของคุณ

ฟีเจอร์หลัก:
- บันทึกข้อมูลความดันโลหิต (SBP/DBP)
- บันทึกข้อมูลน้ำตาลในเลือด
- บันทึกข้อมูลชีพจร
- แสดงกราฟและสถิติ
- ค้นหาข้อมูลตามปฏิทิน
- ส่งรายงานไปยังคลินิก
- Export ข้อมูลเป็น CSV

เหมาะสำหรับ:
- ผู้ป่วยเบาหวาน
- ผู้ป่วยความดันโลหิตสูง
- ผู้ที่ต้องการติดตามสุขภาพ
- ผู้สูงอายุ

ข้อมูลทั้งหมดจะถูกเก็บในอุปกรณ์ของคุณอย่างปลอดภัย
ไม่มีการส่งข้อมูลไปยังเซิร์ฟเวอร์ภายนอก
```

### 4. ข้อมูลกราฟิก
1. **App icon**: อัปโหลดไฟล์ `./assets/icon.png` (512x512)
2. **Feature graphic**: สร้างภาพ 1024x500 pixels
3. **Screenshots**: อย่างน้อย 2 รูป (โทรศัพท์)

### 5. ข้อมูลการจัดหมวดหมู่
1. ไปที่ **"App category"**
2. เลือก:
   - **Category**: Medical
   - **Content rating**: 3+
   - **Target audience**: Adults 18+

### 6. ข้อมูลความปลอดภัย
1. ไปที่ **"App content"**
2. กรอกข้อมูล:
   - **Data safety**: ระบุข้อมูลที่เก็บรวบรวม
   - **Privacy policy**: อัปโหลดไฟล์ Privacy Policy
   - **Target audience**: Adults 18+

### 7. ข้อมูลการชำระเงิน
1. ไปที่ **"Monetization"**
2. เลือก:
   - **Free app**: ✅
   - **In-app purchases**: ❌

## 📋 Checklist ก่อนส่งแอป

### ข้อมูลที่ต้องกรอก
- [ ] ชื่อแอป: จดความดัน&น้ำตาล
- [ ] คำอธิบายสั้นและยาว
- [ ] App icon (512x512)
- [ ] Screenshots (อย่างน้อย 2 รูป)
- [ ] Feature graphic (1024x500)
- [ ] Privacy Policy
- [ ] Data safety information

### ข้อมูลที่ต้องอัปโหลด
- [ ] Android App Bundle (AAB)
- [ ] App icon
- [ ] Screenshots
- [ ] Feature graphic
- [ ] Privacy Policy

## 🔐 ข้อมูลความปลอดภัย

### Data Safety
- **Personal info**: ชื่อ, อีเมล (เก็บในอุปกรณ์)
- **Health & fitness**: ข้อมูลสุขภาพ (เก็บในอุปกรณ์)
- **App activity**: ข้อมูลการใช้งาน (เก็บในอุปกรณ์)
- **Device or other IDs**: ไม่เก็บ

### Privacy Policy
- ข้อมูลถูกเก็บในอุปกรณ์เท่านั้น
- ไม่มีการส่งข้อมูลไปยังเซิร์ฟเวอร์ภายนอก
- ไม่มีการแชร์ข้อมูลกับบุคคลที่สาม

## 📞 การติดต่อ
- **Email**: uradev222@gmail.com
- **GitHub**: https://github.com/prhdev222

---

**หมายเหตุ**: ตรวจสอบข้อมูลล่าสุดจาก Google Play Console
