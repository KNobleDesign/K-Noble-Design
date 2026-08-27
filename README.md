# BuildTrack — Construction & Interior Project Management System

ระบบบริหารจัดการโครงการก่อสร้างและงานตกแต่งภายในครบวงจร (Full-Featured Construction Project & Financial Management Application)

---

## 🌟 ฟีเจอร์หลัก (Key Features)

1. **ระบบบริหารจัดการโครงการ (Project Management & Interactive Gantt)**
   - ผังไทม์ไลน์งาน (Gantt Chart) เชื่อมโยงความคืบหน้าน้ำหนักงาน (Weighted Progress)
   - แผนที่แสดงตำแหน่งโครงการ พร้อมภาพหน้าปกและภาพ 3D Perspective
   - ตัวกรองสถานะโครงการ (Planning, In Progress, Near Completion, Completed, On Hold)

2. **ระบบการเงินและกระแสเงินสด (Financial & Cash Flow Control - Manager Only)**
   - ตรวจสอบงวดชำระเงิน (Installment Milestones & Verification)
   - คำนวณกำไร-ขาดทุน (Profit & Margin), ต้นทุนทางตรง (Base Direct Cost) และค่าแรงช่างตามประเภทงาน (Subcontractor Trade Daily Rates)
   - ระบบความปลอดภัยแยกสิทธิ์ Manager / Engineer / Foreman อย่างเคร่งครัด

3. **ระบบควบคุมคุณภาพและความปลอดภัย (QC & Action Items Manager)**
   - บันทึกรายการตรวจสอบหน้างาน (Defect & QC Inspection) พร้อมอัปโหลดรูปถ่ายหน้างานจริง
   - บันทึกงานเร่งด่วน (Action Items) และการมอบหมายงานรายบุคคล

4. **ระบบจัดการเอกสารและแบบแปลน (Blueprint & Document Repository)**
   - จัดเก็บแบบสถาปัตย์ (ARCH), โครงสร้าง (STR), งานระบบ (MEP), มัณฑนศิลป์ (INT)
   - รองรับไฟล์ PDF, CAD/DWG, BIM, สเปรดชีต และการอัปโหลดไฟล์ภาพแบบแปลนโดยตรง

5. **ระบบจัดการข้อมูลบริษัทและบุคลากร (Company Branding & Personnel)**
   - ปรับแต่งโลโก้บริษัท (Custom Image Upload), ธีมสี (Amber, Emerald, Indigo, Ruby, Slate, Violet), ตราประทับ และข้อมูลทางการ
   - จัดการโปรไฟล์พนักงานและรหัสผ่าน

6. **ระบบพิมพ์รายงานทางการ (A4 Printable Executive Summary)**
   - พิมพ์รายงานสรุปสถานะโครงการสำหรับส่งผู้บริหารหรือเจ้าของโครงการในรูปแบบ A4 สะอาดตา

---

## 🔐 บัญชีเข้าใช้งานระบบเริ่มต้น (Default User Accounts)

| บทบาท (Role) | ชื่อผู้ใช้งาน (Username) | รหัสผ่าน (Password) | สิทธิ์การเข้าถึง |
| :--- | :--- | :--- | :--- |
| **Manager (ผู้จัดการ)** | `manager` หรือ `Somchai Prasert` | `39921` หรือ `somchai@buildtrack.com` | เข้าถึงข้อมูลการเงิน, กำไร, ต้นทุน, บัญชีผู้ใช้, ข้อมูลบริษัท |
| **Engineer (วิศวกร)** | `Wichai Thongdee` | `wichai@buildtrack.com` | จัดการงานไทม์ไลน์, เอกสารแบบแปลน, QC, งวดงาน |
| **Foreman (โฟร์แมน)** | `Anan Suksamran` | `anan@buildtrack.com` | ตรวจสอบหน้างาน, บันทึก QC และ Action Items |

*(หมายเหตุ: สามารถเปลี่ยนรหัสผ่านหรือเพิ่มบัญชีพนักงานใหม่ได้ที่เมนู "ตั้งค่าระบบ")*

---

## 🚀 วิธีการติดตั้งและรันโปรเจกต์ (Installation & Running)

### 1. ติดตั้ง Dependencies
```bash
npm install
```

### 2. รันในโหมด Development
```bash
npm run dev
```
เปิดบราวเซอร์ไปที่ `http://localhost:3000`

### 3. ตรวจสอบโค้ด (Linting)
```bash
npm run lint
```

### 4. สั่ง Build สำหรับ Production
```bash
npm run build
```

---

## 🛠️ โครงสร้างเทคโนโลยี (Tech Stack)
- **Frontend Framework**: React 18+ (TypeScript)
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Persistence**: Local Storage Engine with Automatic Hydration & Data Compression
