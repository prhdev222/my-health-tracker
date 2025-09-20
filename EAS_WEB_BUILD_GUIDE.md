# คู่มือการสร้าง Android App Bundle ผ่าน EAS Web

## 🚀 วิธีที่ 1: ใช้ EAS Web Interface

### ขั้นตอนที่ 1: เข้า EAS Dashboard
1. ไปที่ https://expo.dev
2. Login ด้วยบัญชี prhdev222
3. เลือกโปรเจค "my-health-tracker"

### ขั้นตอนที่ 2: สร้าง Build
1. คลิก "Builds" ในเมนูซ้าย
2. คลิก "Create a build"
3. เลือก:
   - **Platform**: Android
   - **Profile**: production
   - **Workflow**: EAS Build
4. คลิก "Create build"

### ขั้นตอนที่ 3: รอ Build เสร็จ
- ใช้เวลาประมาณ 10-15 นาที
- จะได้ Android App Bundle (.aab) ไฟล์

## 🚀 วิธีที่ 2: ใช้ GitHub Actions (แนะนำ)

### ขั้นตอนที่ 1: เตรียม GitHub Repository
1. สร้าง repository ใหม่ใน GitHub
2. อัปโหลดโค้ดทั้งหมด
3. ตั้งค่า Secrets:
   - `EXPO_TOKEN`: Token จาก expo.dev

### ขั้นตอนที่ 2: ตั้งค่า Expo Token
1. ไปที่ https://expo.dev/settings/access-tokens
2. สร้าง token ใหม่
3. คัดลอก token
4. ไปที่ GitHub Repository > Settings > Secrets and variables > Actions
5. เพิ่ม secret ชื่อ `EXPO_TOKEN`

### ขั้นตอนที่ 3: Push โค้ด
```bash
git add .
git commit -m "Add Android build workflow"
git push origin main
```

## 📱 ข้อมูลแอปสำหรับ Google Play Store

### ข้อมูลพื้นฐาน
- **ชื่อแอป**: จดความดัน&น้ำตาล
- **Package Name**: com.myhealthtracker.app
- **Version**: 1.0.0
- **Version Code**: 1

### คำอธิบายแอป
**คำอธิบายสั้น** (80 ตัวอักษร):
```
แอปติดตามข้อมูลสุขภาพส่วนตัว
```

**คำอธิบายยาว**:
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

### ข้อมูลการจัดหมวดหมู่
- **หมวดหมู่**: Medical
- **เนื้อหา**: 3+ (สำหรับทุกวัย)
- **กลุ่มเป้าหมาย**: ผู้ใหญ่ 18+

### ข้อมูลการชำระเงิน
- **แอปฟรี**: ใช่
- **มี In-App Purchase**: ไม่

## 🎨 Assets ที่ต้องเตรียม

### App Icon
- **ขนาด**: 512x512 pixels
- **รูปแบบ**: PNG
- **ไฟล์**: `./assets/icon.png` (มีอยู่แล้ว)

### Screenshots
ต้องเตรียม screenshots สำหรับ:
- **โทรศัพท์**: อย่างน้อย 2 รูป
- **แท็บเล็ต**: อย่างน้อย 1 รูป (ถ้ามี)

### Feature Graphic
- **ขนาด**: 1024x500 pixels
- **รูปแบบ**: PNG หรือ JPG

## 🔐 ข้อมูลความปลอดภัย

### Permissions
แอปใช้ permissions ดังนี้:
- `android.permission.INTERNET` - สำหรับส่งอีเมล
- `android.permission.ACCESS_NETWORK_STATE` - ตรวจสอบสถานะเครือข่าย

### Data Safety
- **Personal info**: ชื่อ, อีเมล (เก็บในอุปกรณ์)
- **Health & fitness**: ข้อมูลสุขภาพ (เก็บในอุปกรณ์)
- **App activity**: ข้อมูลการใช้งาน (เก็บในอุปกรณ์)
- **Device or other IDs**: ไม่เก็บ

## 📝 ขั้นตอนการอัปโหลดไป Google Play Store

### 1. สร้าง Google Play Console Account
- ไปที่ https://play.google.com/console
- สร้างบัญชีผู้พัฒนา (ต้องเสียค่าธรรมเนียม $25)

### 2. สร้างแอปใหม่
- คลิก "Create app"
- กรอกข้อมูล:
  - **App name**: จดความดัน&น้ำตาล
  - **Default language**: Thai (ไทย)
  - **App or game**: App
  - **Free or paid**: Free

### 3. อัปโหลด AAB
- ไปที่ "Release" > "Production"
- อัปโหลดไฟล์ AAB ที่สร้างจาก EAS

### 4. กรอกข้อมูลแอป
- ข้อมูลแอป (ชื่อ, คำอธิบาย)
- ข้อมูลกราฟิก (icon, screenshots)
- ข้อมูลการจัดหมวดหมู่
- Privacy Policy

### 5. ตรวจสอบและส่ง
- ตรวจสอบข้อมูลทั้งหมด
- ส่งแอปเพื่อตรวจสอบ

## ⏰ ระยะเวลาการตรวจสอบ
- **ครั้งแรก**: 1-3 วัน
- **อัปเดต**: 1-2 วัน

## 📞 การติดต่อ
- **Email**: uradev222@gmail.com
- **GitHub**: https://github.com/prhdev222

---

**หมายเหตุ**: วิธีที่ 2 (GitHub Actions) เป็นวิธีที่แนะนำเพราะจะแก้ปัญหา filename casing ได้
