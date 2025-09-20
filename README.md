# My Health Tracker 📱

แอปพลิเคชันสำหรับติดตามข้อมูลสุขภาพส่วนตัว พัฒนาด้วย React Native และ Expo

## ✨ ฟีเจอร์หลัก

- 📊 **บันทึกข้อมูลสุขภาพ**
  - ความดันโลหิต (Systolic/Diastolic)
  - ระดับน้ำตาลในเลือด
  - อัตราการเต้นของหัวใจ

- 📈 **แสดงกราฟและสถิติ**
  - กราฟแยกตามประเภทข้อมูล
  - สถิติเฉลี่ย, สูงสุด, ต่ำสุด
  - กราฟรายวัน, รายสัปดาห์, รายเดือน

- 🔍 **ค้นหาข้อมูล**
  - ค้นหาตามคำสำคัญ
  - ค้นหาตามปฏิทิน
  - แสดงวงสีในวันที่มีข้อมูล

- 📧 **ส่งรายงาน**
  - ส่งข้อมูลไปยังคลินิก
  - รูปแบบตารางสวยงาม
  - ข้อมูล 3 เดือนล่าสุด

- 💾 **Export ข้อมูล**
  - ดาวน์โหลดเป็นไฟล์ CSV
  - เลือกช่วงเวลาได้
  - แยกข้อมูลตามประเภท

## 🚀 การติดตั้ง

### ข้อกำหนดระบบ
- Node.js 16+
- npm หรือ yarn
- Expo CLI
- Android Studio (สำหรับ Android)
- Xcode (สำหรับ iOS)

### ขั้นตอนการติดตั้ง

1. **Clone repository**
   ```bash
   git clone https://github.com/yourusername/my-health-tracker.git
   cd my-health-tracker
   ```

2. **ติดตั้ง dependencies**
   ```bash
   npm install
   ```

3. **เริ่มต้นแอป**
   ```bash
   npm start
   ```

4. **รันบนอุปกรณ์**
   - Android: `npm run android`
   - iOS: `npm run ios`
   - Web: `npm run web`

## 📱 การใช้งาน

### หน้าหลัก
- กรอกข้อมูลความดันโลหิต
- กรอกข้อมูลน้ำตาลในเลือด
- กรอกข้อมูลชีพจร
- บันทึกข้อมูล

### หน้าประวัติ
- ดูกราฟข้อมูล
- ค้นหาข้อมูล
- ดูสถิติ
- Export ข้อมูล

### หน้าตั้งค่า
- ตั้งค่าข้อมูลผู้ป่วย
- ตั้งค่าข้อมูลคลินิก
- จัดการข้อมูล

## 🛠️ การพัฒนา

### โครงสร้างโปรเจค
```
src/
├── database/          # ฐานข้อมูล SQLite
├── screens/           # หน้าจอต่างๆ
├── services/          # บริการต่างๆ
└── types/            # TypeScript types
```

### การ Build สำหรับ Production

1. **ติดตั้ง EAS CLI**
   ```bash
   npm install -g eas-cli
   ```

2. **Login เข้า Expo**
   ```bash
   eas login
   ```

3. **Build Android**
   ```bash
   npm run build:android
   ```

4. **Build Preview**
   ```bash
   npm run build:android-preview
   ```

## 📋 ข้อมูลสำหรับ Google Play Store

- **Package Name**: com.myhealthtracker.app
- **Version**: 1.0.0
- **Version Code**: 1
- **Target SDK**: 34
- **Min SDK**: 21

## 🔒 ความปลอดภัย

- ข้อมูลถูกเก็บในฐานข้อมูล SQLite ในอุปกรณ์
- ไม่มีการส่งข้อมูลไปยังเซิร์ฟเวอร์ภายนอก
- ข้อมูลจะไม่ถูกแชร์กับบุคคลที่สาม

## 📄 License

MIT License - ดูรายละเอียดในไฟล์ [LICENSE](LICENSE)

## 🤝 การมีส่วนร่วม

1. Fork โปรเจค
2. สร้าง feature branch
3. Commit การเปลี่ยนแปลง
4. Push ไปยัง branch
5. สร้าง Pull Request

## 📞 การติดต่อ

- **Email**: [your-email@example.com]
- **GitHub**: [https://github.com/yourusername/my-health-tracker]

## 🙏 การขอบคุณ

- React Native
- Expo
- React Navigation
- React Native Chart Kit
- React Native Calendars

---

**หมายเหตุ**: แอปนี้เหมาะสำหรับการติดตามข้อมูลสุขภาพส่วนตัว ไม่ควรใช้แทนการปรึกษาแพทย์

## Build Status
- Android production build ready
- Triggering build for Google Play Store