# Day05 — GitHub, Markdown, README, Developer Tools & Learning Portfolio
## แผนสอนและปฏิบัติ 1 ชั่วโมง 30 นาที สำหรับนักศึกษาใหม่วิศวกรรมซอฟต์แวร์
### Platform: Windows + VS Code สำหรับแก้ไขไฟล์ + Git command line ผ่าน CMD

> แนวทางสำคัญ: ยังไม่เชื่อม VS Code กับ GitHub เพื่อไม่ให้ซับซ้อนเกินไปในคาบแรก  
> ใช้ VS Code เพื่อเปิดโฟลเดอร์ แก้ไขไฟล์ และบันทึกเท่านั้น  
> ใช้ CMD เพื่อฝึกคำสั่ง Git จริง  
> ใช้ GitHub Website เพื่อสร้าง repository และตรวจผลลัพธ์

---

## 1. แนวคิดของกิจกรรม

กิจกรรมนี้ออกแบบสำหรับนักศึกษาใหม่ที่ **ไม่มีพื้นฐาน Git/GitHub มาก่อน** โดยเน้นให้ทุกคนทำสำเร็จจริงภายใน 1 ชั่วโมง 30 นาที และมีผลงานที่เปิดดูได้บน GitHub

สิ่งที่นักศึกษาจะทำได้เมื่อจบคาบ:

1. สร้างโฟลเดอร์ project บน Windows
2. เปิดโฟลเดอร์ด้วย VS Code
3. สร้างและแก้ไขไฟล์ `README.md`
4. เขียน Markdown พื้นฐาน
5. ใช้คำสั่ง Git ผ่าน CMD
6. commit งานแรกในเครื่อง
7. สร้าง GitHub repository แรก
8. push งานจากเครื่องขึ้น GitHub
9. ได้ GitHub Learning Portfolio เบื้องต้น

---

## 2. เป้าหมายการเรียนรู้

หลังจบกิจกรรม นักศึกษาควรสามารถ:

1. อธิบายความแตกต่างระหว่าง Git และ GitHub ได้
2. เข้าใจคำว่า repository, README, commit, remote, push ในระดับเริ่มต้น
3. สร้าง README.md ด้วย Markdown ได้
4. ใช้ VS Code เพื่อแก้ไขและ preview Markdown ได้
5. ใช้ CMD เพื่อสั่ง `git init`, `git status`, `git add`, `git commit`, `git remote`, `git push` ได้
6. สร้าง GitHub repository แรกได้
7. ส่ง repository URL ให้อาจารย์ได้
8. ใช้ GitHub เป็นพื้นที่สะสมหลักฐานการเรียนรู้ได้

---

## 3. สิ่งที่ต้องเตรียม

### 3.1 สำหรับผู้สอน

- เครื่อง Windows สำหรับสาธิต
- Projector
- Internet
- Git for Windows ติดตั้งแล้ว
- Visual Studio Code ติดตั้งแล้ว
- Browser เช่น Chrome หรือ Edge
- GitHub account ตัวอย่าง
- README template
- Google Form หรือ QR Code สำหรับส่ง repository link

### 3.2 สำหรับนักศึกษา

- Email ที่ใช้งานได้
- GitHub account หรือพร้อมสมัคร
- เครื่อง Windows ที่มี Git และ VS Code
- Internet
- สมุดจดหรือไฟล์จดคำสั่ง

---

## 4. โครงเวลา 1 ชั่วโมง 30 นาที

| เวลา | กิจกรรม | ผลลัพธ์ |
|---:|---|---|
| 0–10 นาที | ภาพรวม Git, GitHub, Portfolio | เข้าใจว่าทำไปเพื่ออะไร |
| 10–20 นาที | ตรวจ GitHub account, Git, VS Code | พร้อมลงมือ |
| 20–35 นาที | สร้างโฟลเดอร์และ README.md | ได้ README.md ในเครื่อง |
| 35–50 นาที | ใช้ Git local: init, status, add, commit | ได้ commit แรก |
| 50–65 นาที | สร้าง GitHub repo และ push | งานขึ้น GitHub |
| 65–80 นาที | ปรับ README เป็น Learning Portfolio | portfolio ชัดขึ้น |
| 80–90 นาที | ตรวจ checklist, ส่ง link, exit ticket | ส่งผลงานได้ |

---

# Part A — เนื้อหาสอนก่อนลงมือ

## 5. GitHub คืออะไร

GitHub คือพื้นที่ออนไลน์สำหรับเก็บ repository และแสดงผลงานของนักพัฒนา software

สำหรับนักศึกษาใหม่ GitHub ใช้เพื่อ:

- เก็บงาน lab และ project
- แสดง README และ portfolio
- ติดตามพัฒนาการของตนเอง
- ฝึก workflow ของนักพัฒนาซอฟต์แวร์
- เตรียมหลักฐานสำหรับฝึกงาน สมัครงาน หรือ capstone project

ประโยคที่ควรย้ำ:

> GitHub ไม่ใช่แค่ที่เก็บ code แต่เป็นพื้นที่แสดงหลักฐานการเรียนรู้ของนักศึกษา Software Engineering

---

## 6. Git กับ GitHub ต่างกันอย่างไร

| ประเด็น | Git | GitHub |
|---|---|---|
| คืออะไร | โปรแกรม version control | เว็บไซต์สำหรับเก็บ Git repository ออนไลน์ |
| อยู่ที่ไหน | เครื่องของเรา | บนเว็บ |
| ใช้ทำอะไร | บันทึกประวัติการเปลี่ยนแปลง | แชร์ เก็บ แสดงผลงาน และทำงานร่วมกัน |
| ตัวอย่าง | `git init`, `git commit` | create repository, view README |
| เปรียบเทียบ | สมุดบันทึกประวัติในเครื่อง | ชั้นวางผลงานออนไลน์ |

---

## 7. คำศัพท์พื้นฐาน

| คำศัพท์ | ความหมายแบบง่าย |
|---|---|
| Repository / repo | โฟลเดอร์ project ที่ Git ติดตามการเปลี่ยนแปลง |
| README.md | ไฟล์แนะนำ project ที่ GitHub แสดงหน้าแรก |
| Markdown | รูปแบบเขียนเอกสาร plain text ให้แสดงผลสวยบน GitHub |
| Commit | จุดบันทึกการเปลี่ยนแปลง |
| Remote | repository ปลายทางบน GitHub |
| Push | ส่ง commit จากเครื่องขึ้น GitHub |
| Status | ตรวจว่าไฟล์มีการเปลี่ยนแปลงอะไรบ้าง |

---

## 8. Markdown คืออะไร

Markdown คือรูปแบบการเขียนเอกสารแบบ plain text ที่อ่านง่าย และ GitHub สามารถแสดงผลให้สวยงามได้

ตัวอย่าง Markdown พื้นฐาน:

```markdown
# หัวข้อใหญ่

## หัวข้อย่อย

- รายการที่ 1
- รายการที่ 2

**ตัวหนา**

[GitHub](https://github.com)

| หัวข้อ | รายละเอียด |
|---|---|
| Tool | GitHub |
```

สิ่งที่ควรรู้ในคาบนี้:

| Markdown | ใช้ทำอะไร |
|---|---|
| `#` | หัวข้อใหญ่ |
| `##` | หัวข้อย่อย |
| `-` | bullet list |
| `**text**` | ตัวหนา |
| `[text](url)` | link |
| `` `code` `` | code สั้น |
| code block | แสดงคำสั่งหลายบรรทัด |
| table | ตาราง |

---

## 9. README.md คืออะไร

`README.md` คือไฟล์ที่ GitHub แสดงเป็นหน้าแรกของ repository

README ที่ดีควรตอบ:

1. Project นี้คืออะไร
2. ทำไปเพื่ออะไร
3. มีอะไรอยู่ใน repository นี้
4. วิธีใช้งานหรือเปิดดูคืออะไร
5. เจ้าของ project คือใคร
6. ได้เรียนรู้อะไร
7. จะพัฒนาต่ออย่างไร

สำหรับกิจกรรมนี้ README จะเป็น **Learning Portfolio เบื้องต้น** ของนักศึกษา

---

# Part B — Step-by-step Workshop บน Windows

## 10. Workflow ที่จะทำในคาบนี้

```text
สร้างโฟลเดอร์ในเครื่อง
  ↓
เปิดโฟลเดอร์ด้วย VS Code
  ↓
สร้าง README.md
  ↓
เขียน Markdown และบันทึก
  ↓
เปิด CMD
  ↓
git init
  ↓
git add README.md
  ↓
git commit
  ↓
สร้าง repo บน GitHub
  ↓
git remote add origin ...
  ↓
git push
  ↓
เปิด GitHub ดูผลงาน
```

---

## 11. Step 0 — ตรวจความพร้อม

### 11.1 ตรวจ Git

เปิด Command Prompt หรือ CMD แล้วพิมพ์:

```cmd
git --version
```

ผลลัพธ์ที่คาดหวัง:

```cmd
git version 2.xx.x.windows.x
```

ถ้าไม่พบคำสั่ง `git` ให้แจ้งผู้สอน

---

### 11.2 ตรวจ VS Code

เปิด Start Menu แล้วค้นหา:

```text
Visual Studio Code
```

หรือพิมพ์ใน CMD:

```cmd
code --version
```

ถ้าใช้คำสั่ง `code` ไม่ได้ ไม่เป็นไร ให้เปิด VS Code จาก Start Menu แทน

---

### 11.3 ตรวจ GitHub Account

ให้นักศึกษาเปิด browser ไปที่ GitHub และ login

ตรวจว่า:

- login ได้
- จำ username ได้
- email ใช้งานได้
- ถ้ามีการยืนยันตัวตน ให้ทำตามขั้นตอนบนหน้าจอ

---

## 12. Step 1 — ตั้งค่า Git ครั้งแรก

ใน CMD พิมพ์คำสั่งต่อไปนี้ โดยเปลี่ยนชื่อและ email เป็นของตนเอง:

```cmd
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
git config --global init.defaultBranch main
```

ตรวจค่าที่ตั้งไว้:

```cmd
git config --list
```

หรือดูทีละค่า:

```cmd
git config user.name
git config user.email
```

คำอธิบาย:

| คำสั่ง | ความหมาย |
|---|---|
| `user.name` | ชื่อที่จะแสดงใน commit |
| `user.email` | email ที่ผูกกับ commit |
| `init.defaultBranch main` | ให้ branch เริ่มต้นชื่อ `main` |

---

## 13. Step 2 — สร้างโฟลเดอร์ Project

ใน CMD พิมพ์:

```cmd
cd %USERPROFILE%\Documents
mkdir se-bootcamp-portfolio
cd se-bootcamp-portfolio
```

ตรวจว่าอยู่ถูกโฟลเดอร์:

```cmd
cd
```

ผลลัพธ์ควรเป็น path ประมาณนี้:

```cmd
C:\Users\YourName\Documents\se-bootcamp-portfolio
```

---

## 14. Step 3 — เปิดโฟลเดอร์ด้วย VS Code

ถ้าคำสั่ง `code` ใช้ได้ ให้พิมพ์:

```cmd
code .
```

ถ้าใช้ไม่ได้ ให้เปิดเอง:

1. เปิด Visual Studio Code
2. เลือก `File`
3. เลือก `Open Folder...`
4. ไปที่ `Documents`
5. เลือก `se-bootcamp-portfolio`
6. กด `Select Folder`

---

## 15. Step 4 — สร้างไฟล์ README.md

ใน VS Code:

1. คลิกขวาที่พื้นที่ Explorer
2. เลือก `New File`
3. ตั้งชื่อไฟล์ว่า `README.md`
4. กด Enter
5. คัดลอก template ด้านล่างไปวาง
6. แก้ข้อมูลเป็นของตนเอง
7. กด `Ctrl + S` เพื่อบันทึก

---

## 16. README Template สำหรับนักศึกษาใหม่

```markdown
# My SE Bootcamp Learning Portfolio

## About Me
- Name:
- Nickname:
- Background: ม.6 / ปวช. / ปวส.
- Interest: Web / Mobile / AI / Game / IoT / Data / UX/UI / ยังไม่แน่ใจ

## Why I Study Software Engineering
เขียนสั้น ๆ ว่าทำไมถึงสนใจเรียนสาขานี้

## What I Learned in SE Bootcamp

### Day 01: Digital Foundation
- ฉันได้เรียนรู้ว่า...

### Day 02: Logic & Flowgorithm Lab 1
- ฉันได้เรียนรู้ว่า...

### Day 03: Flowgorithm Lab 2-3
- ฉันได้เรียนรู้ว่า...

### Day 04: AI, Web Technology and Network
- ฉันได้เรียนรู้ว่า...

### Day 05: GitHub and Developer Tools
- ฉันได้เรียนรู้ว่า...

## My Flowgorithm Labs
- Pass / Fail
- Grade Calculator
- Average Score

## AI Usage Note
ฉันใช้ AI ช่วยเรื่อง...
ฉันตรวจสอบคำตอบของ AI โดย...

## My Learning Goal
เป้าหมายใน 1 เดือนแรกของการเรียนคือ...

## Reflection
สิ่งที่ฉันยังต้องฝึกต่อคือ...
```

---

## 17. Step 5 — Preview Markdown ใน VS Code

วิธีดูตัวอย่าง Markdown:

1. เปิดไฟล์ `README.md`
2. กด `Ctrl + Shift + V`

หรือ:

1. คลิกขวาที่ไฟล์
2. เลือก `Open Preview`

ตรวจว่า:

- หัวข้อแสดงถูกต้อง
- bullet list แสดงถูกต้อง
- link แสดงถูกต้อง
- ไม่มีข้อความติดกันจนอ่านยาก

---

## 18. Step 6 — สร้าง Git Repository ในเครื่อง

กลับไปที่ CMD:

```cmd
cd %USERPROFILE%\Documents\se-bootcamp-portfolio
```

เริ่มต้น Git repository:

```cmd
git init
```

ตรวจสถานะ:

```cmd
git status
```

สิ่งที่ควรเห็น:

- มีไฟล์ `README.md` เป็น untracked file

---

## 19. Step 7 — เพิ่มไฟล์เข้า staging area

พิมพ์:

```cmd
git add README.md
```

ตรวจสถานะอีกครั้ง:

```cmd
git status
```

ควรเห็นว่า `README.md` อยู่ในสถานะที่จะ commit

---

## 20. Step 8 — สร้าง Commit แรก

พิมพ์:

```cmd
git commit -m "Add initial learning portfolio"
```

ตรวจ log:

```cmd
git log --oneline
```

ควรเห็น commit 1 รายการ เช่น:

```cmd
a1b2c3d Add initial learning portfolio
```

---

## 21. Step 9 — สร้าง Repository บน GitHub

ใน browser:

1. เข้า GitHub
2. กดปุ่ม `+` มุมขวาบน
3. เลือก `New repository`
4. Repository name ใช้ชื่อ:

```text
se-bootcamp-portfolio
```

5. Description ใส่ได้ เช่น:

```text
My first Software Engineering learning portfolio
```

6. เลือก Public หรือ Private ตามที่อาจารย์กำหนด
7. **ไม่ต้องเลือก Add README**
8. ไม่ต้องเลือก `.gitignore`
9. ไม่ต้องเลือก license
10. กด `Create repository`

เหตุผลที่ไม่เลือก Add README: เพราะเราสร้าง `README.md` ในเครื่องแล้ว ถ้า GitHub สร้างให้อีก อาจทำให้ push ครั้งแรกยุ่งยากสำหรับนักศึกษาใหม่

---

## 22. Step 10 — เชื่อม Local Repository กับ GitHub

หลังสร้าง repo แล้ว ให้คัดลอก URL เช่น:

```text
https://github.com/USERNAME/se-bootcamp-portfolio.git
```

ใน CMD พิมพ์ โดยเปลี่ยน `USERNAME` เป็น username ของตนเอง:

```cmd
git remote add origin https://github.com/USERNAME/se-bootcamp-portfolio.git
git branch -M main
git push -u origin main
```

ระหว่าง push อาจมีหน้าต่างให้ login GitHub หรือ browser เปิดขึ้นมา ให้ทำตามขั้นตอนบนหน้าจอ

---

## 23. Step 11 — ตรวจผลบน GitHub

หลัง push สำเร็จ:

1. กลับไปที่หน้า repository บน GitHub
2. refresh หน้าเว็บ
3. ควรเห็นไฟล์ `README.md`
4. GitHub ควรแสดงเนื้อหา README เป็นหน้า portfolio
5. Copy URL ของ repository ส่งให้อาจารย์

ตัวอย่าง URL:

```text
https://github.com/USERNAME/se-bootcamp-portfolio
```

---

## 24. Step 12 — แก้ README เพิ่มเติมและ commit รอบที่ 2

กลับไปที่ VS Code แล้วปรับ README ให้สมบูรณ์ขึ้น

หลังแก้ไขแล้วกด `Ctrl + S`

ใน CMD:

```cmd
git status
git add README.md
git commit -m "Improve README learning portfolio"
git push
```

กลับไปตรวจบน GitHub ว่า README เปลี่ยนแล้ว

---

# Part C — กิจกรรม Interactive ในห้องเรียน

## 25. กิจกรรมที่ 1: Git Command Card Sort

**เวลา:** 5 นาที  
**รูปแบบ:** จับคู่หรือกลุ่ม 3 คน

ให้นักศึกษาจัดลำดับคำสั่งต่อไปนี้ให้ถูกต้อง:

```cmd
git commit -m "Add initial learning portfolio"
git init
git push -u origin main
git add README.md
git remote add origin https://github.com/USERNAME/se-bootcamp-portfolio.git
git status
```

เฉลย:

```cmd
git init
git status
git add README.md
git commit -m "Add initial learning portfolio"
git remote add origin https://github.com/USERNAME/se-bootcamp-portfolio.git
git push -u origin main
```

---

## 26. กิจกรรมที่ 2: Markdown Fix

ให้นักศึกษาดู Markdown ที่เขียนผิด แล้วแก้ให้ถูก

ตัวอย่างผิด:

```markdown
#My Portfolio
##About Me
-Name: Somchai
-Interest: Web
```

แก้ให้ถูก:

```markdown
# My Portfolio

## About Me
- Name: Somchai
- Interest: Web
```

---

## 27. กิจกรรมที่ 3: Portfolio Pair Review

ให้นักศึกษาจับคู่แลก repository link แล้วตรวจตาม checklist:

1. เปิด repository ได้หรือไม่
2. README แสดงผลหรือไม่
3. มี About Me หรือไม่
4. มี What I Learned หรือไม่
5. มี Learning Goal หรือไม่
6. อ่านแล้วเข้าใจเจ้าของ portfolio หรือไม่
7. มีจุดใดที่ควรปรับให้ชัดขึ้น

---

## 28. Exit Ticket

ให้นักศึกษาส่งคำตอบสั้น ๆ ผ่าน Google Form หรือกระดาษ:

1. วันนี้ฉันได้เรียนรู้คำสั่ง Git อะไรบ้าง
2. คำสั่งใดที่ยังไม่มั่นใจ
3. GitHub portfolio ของฉันคือ URL อะไร
4. README ของฉันยังต้องปรับอะไรต่อ
5. เป้าหมายการฝึกต่อใน 1 สัปดาห์คืออะไร

---

# Part D — Checklist ผลงาน

| รายการ | สถานะ |
|---|---|
| เข้า GitHub account ได้ | ☐ |
| สร้างโฟลเดอร์ `se-bootcamp-portfolio` ได้ | ☐ |
| สร้างไฟล์ `README.md` ได้ | ☐ |
| เขียน Markdown อย่างน้อย 5 รูปแบบได้ | ☐ |
| preview Markdown ใน VS Code ได้ | ☐ |
| ใช้ `git init` ได้ | ☐ |
| ใช้ `git add` ได้ | ☐ |
| ใช้ `git commit` ได้ | ☐ |
| สร้าง GitHub repository ได้ | ☐ |
| ใช้ `git remote add origin` ได้ | ☐ |
| ใช้ `git push` ได้ | ☐ |
| เปิด GitHub แล้วเห็น README ได้ | ☐ |
| ส่ง repository link ให้อาจารย์ได้ | ☐ |

---

# Part E — Troubleshooting

## 29. `git` ไม่เป็นที่รู้จัก

อาการ:

```cmd
'git' is not recognized as an internal or external command
```

แนวทางแก้:

- ตรวจว่า Git for Windows ติดตั้งแล้วหรือไม่
- ปิด CMD แล้วเปิดใหม่
- หากยังไม่ได้ แจ้งผู้สอนตรวจ PATH หรือเครื่อง lab

---

## 30. Commit ไม่ได้เพราะยังไม่ได้ตั้งชื่อ/email

แก้ด้วย:

```cmd
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

แล้วลอง commit อีกครั้ง

---

## 31. `nothing to commit`

ความหมาย:

- ไม่มีไฟล์ใหม่หรือไฟล์ที่แก้ไขแล้วให้ commit
- อาจ commit ไปแล้ว
- หรือยังไม่ได้บันทึกไฟล์ใน VS Code

ตรวจด้วย:

```cmd
git status
```

---

## 32. `remote origin already exists`

ตรวจ remote:

```cmd
git remote -v
```

แก้ URL ใหม่:

```cmd
git remote set-url origin https://github.com/USERNAME/se-bootcamp-portfolio.git
```

---

## 33. Push ไม่ผ่านเพราะ repo บน GitHub มี README อยู่แล้ว

สาเหตุที่พบบ่อยคือ ตอนสร้าง repo บน GitHub เลือก Add README ไว้

สำหรับนักศึกษาใหม่ วิธีง่ายที่สุด:

1. สร้าง repository ใหม่อีกครั้ง
2. ไม่เลือก Add README
3. push ใหม่ตามขั้นตอน

---

## 34. Login GitHub ตอน push ไม่ผ่าน

แนวทาง:

- ตรวจ internet
- ตรวจว่า login GitHub ใน browser ได้
- ถ้ามีหน้าต่าง sign-in ให้ทำตามขั้นตอน
- ถ้าใช้เครื่อง lab ร่วมกัน หลังจบกิจกรรมควร sign out จาก browser และไม่บันทึกรหัสผ่านในเครื่องสาธารณะ
- หากยัง push ไม่ได้ ให้ส่งไฟล์ `README.md` ให้อาจารย์ก่อน แล้วแก้เรื่อง authentication ภายหลัง

---

# Part F — Post-test ตัวอย่าง

## ข้อ 1

Git คืออะไร

A. เว็บไซต์สำหรับดูวิดีโอ  
B. เครื่องมือจัดการ version และประวัติการเปลี่ยนแปลงของไฟล์  
C. โปรแกรมวาดรูป  
D. ฐานข้อมูล  

**เฉลย:** B

---

## ข้อ 2

GitHub คืออะไร

A. เว็บไซต์สำหรับเก็บและแชร์ Git repository ออนไลน์  
B. โปรแกรมแก้ไขรูปภาพ  
C. ระบบปฏิบัติการ  
D. ภาษาโปรแกรม  

**เฉลย:** A

---

## ข้อ 3

ไฟล์ใดที่ GitHub มักแสดงเป็นหน้าแรกของ repository

A. `main.exe`  
B. `README.md`  
C. `photo.jpg`  
D. `system32.dll`  

**เฉลย:** B

---

## ข้อ 4

คำสั่งใดใช้เริ่ม Git repository ในโฟลเดอร์ปัจจุบัน

A. `git start`  
B. `git init`  
C. `git open`  
D. `git create github`  

**เฉลย:** B

---

## ข้อ 5

คำสั่งใดใช้บันทึกการเปลี่ยนแปลงเป็น commit

A. `git save`  
B. `git commit -m "message"`  
C. `git send`  
D. `git upload now`  

**เฉลย:** B

---

## ข้อ 6

คำสั่งใดใช้ส่ง commit จากเครื่องขึ้น GitHub

A. `git push`  
B. `git pull`  
C. `git read`  
D. `git show web`  

**เฉลย:** A

---

# Part G — Output ที่นักศึกษาต้องส่ง

ให้นักศึกษาส่ง:

1. GitHub repository URL
2. Screenshot หน้า repository ที่เห็น README
3. คำตอบ Exit Ticket
4. Checklist ที่ทำสำเร็จ
5. ถ้า push ไม่สำเร็จ ให้ส่งไฟล์ `README.md` ชั่วคราวก่อน

ตัวอย่าง repository URL:

```text
https://github.com/USERNAME/se-bootcamp-portfolio
```

---

# Part H — สรุปท้ายกิจกรรมสำหรับอาจารย์

> วันนี้นักศึกษาไม่ได้แค่สมัคร GitHub หรือสร้าง README แต่ได้เริ่มฝึก workflow ของนักพัฒนาซอฟต์แวร์จริง คือ เขียนเอกสาร แก้ไขไฟล์ ตรวจสถานะ บันทึก commit และส่งผลงานขึ้น repository ออนไลน์ ต่อไป GitHub จะเป็นพื้นที่สะสมหลักฐานการเรียนรู้และพัฒนาการของนักศึกษาในสาขาวิศวกรรมซอฟต์แวร์

---

# Part I — แหล่งอ้างอิงสำหรับผู้สอน

- Git official website: https://git-scm.com/
- Pro Git Book — First-Time Git Setup: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
- GitHub Docs — Quickstart for repositories: https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories
- GitHub Docs — Adding locally hosted code to GitHub: https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github
- GitHub Docs — Basic writing and formatting syntax: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
- VS Code Docs — Markdown and Visual Studio Code: https://code.visualstudio.com/docs/languages/markdown
