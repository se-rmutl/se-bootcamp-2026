# Day 03 — Flowgorithm Lab 2 & Lab 3  
## พุธ 10 มิ.ย. 2569  
**สถานที่:** แยกห้อง  
**เวลา:** 09:00 - 16:00 น.

---

## ภาพรวมของวัน

Day 03 เป็นวันที่ต่อยอดจาก Day 02 โดยเพิ่มความสามารถด้านตรรกะให้ลึกขึ้น นักศึกษาจะได้ฝึกเงื่อนไขหลายกรณี Boolean Logic การเขียน Pseudocode จาก Flowchart การใช้ Loop และการไล่ค่าตัวแปรด้วย Trace Table

ช่วงท้ายของวันจะให้เปิดดู Source Code จาก Flowgorithm เพื่อให้นักศึกษาเห็นภาพว่า flowchart ที่ตนเองสร้างสามารถแปลงไปเป็นภาษาคอมพิวเตอร์จริงได้

```text
Flowchart
  ↓
Pseudocode
  ↓
Run & Test
  ↓
Trace Table
  ↓
Source Code Viewer
  ↓
Mini Demo
```

---

# ช่วงเช้า 09:00 - 12:00 น.  
## Flowgorithm Lab 2: Decision Logic & Pseudocode

## เป้าหมายช่วงเช้า

1. ใช้ If / Else และ Else If ได้
2. เข้าใจ Boolean Logic เช่น AND / OR / NOT
3. เข้าใจเงื่อนไขซ้อนหรือเงื่อนไขหลายกรณี
4. แปลง flowchart เป็น pseudocode ได้
5. คิด test case สำหรับกรณีขอบเขตได้

## โครงสร้างเวลา

| เวลา | กิจกรรม |
|---:|---|
| 09:00 - 09:20 | ทบทวน Lab 1 และ If / Else |
| 09:20 - 10:10 | Lab 3: Grade Calculator |
| 10:10 - 10:30 | Edge Case และ Test Case |
| 10:30 - 10:45 | พัก |
| 10:45 - 11:25 | Boolean Logic: AND / OR / NOT |
| 11:25 - 11:50 | Lab 4: Exam Eligibility |
| 11:50 - 12:00 | สรุปและ Reflection สั้น ๆ |

## Lab 3: Grade Calculator

โจทย์

> รับคะแนน แล้วแสดงเกรด A, B, C, D, F

เกณฑ์ตัวอย่าง

| คะแนน | เกรด |
|---:|---|
| 80 - 100 | A |
| 70 - 79 | B |
| 60 - 69 | C |
| 50 - 59 | D |
| ต่ำกว่า 50 | F |

Pseudocode ตัวอย่าง

```text
INPUT score

IF score >= 80 THEN
    grade = "A"
ELSE IF score >= 70 THEN
    grade = "B"
ELSE IF score >= 60 THEN
    grade = "C"
ELSE IF score >= 50 THEN
    grade = "D"
ELSE
    grade = "F"
ENDIF

DISPLAY grade
```

จุดที่ควรเน้น

- ลำดับการตรวจเงื่อนไขสำคัญมาก
- ถ้าเรียงเงื่อนไขผิด ผลลัพธ์ผิดได้
- ต้องทดสอบคะแนนขอบเขต เช่น 49, 50, 59, 60, 69, 70, 79, 80

Test Case

| Test Case | score | Expected Grade |
|---|---:|---|
| TC01 | 80 | A |
| TC02 | 79 | B |
| TC03 | 70 | B |
| TC04 | 69 | C |
| TC05 | 60 | C |
| TC06 | 59 | D |
| TC07 | 50 | D |
| TC08 | 49 | F |

## Boolean Logic: AND / OR / NOT

| Logic | ความหมาย | ตัวอย่าง |
|---|---|---|
| AND | ต้องจริงทั้งสองเงื่อนไข | attendance >= 80 AND submittedWork == true |
| OR | จริงอย่างน้อยหนึ่งเงื่อนไข | member == true OR coupon == true |
| NOT | กลับค่าจริง/เท็จ | NOT isValid |

## Lab 4: Exam Eligibility

โจทย์

> นักศึกษามีสิทธิ์เข้าสอบเมื่อมีเวลาเรียนไม่น้อยกว่า 80% และส่งงานครบ

Logic

```text
IF attendance >= 80 AND submittedWork == true THEN
    DISPLAY "Eligible"
ELSE
    DISPLAY "Not eligible"
ENDIF
```

Truth Table

| attendance >= 80 | submittedWork | Expected Output |
|---|---|---|
| true | true | Eligible |
| true | false | Not eligible |
| false | true | Not eligible |
| false | false | Not eligible |

## การปรับกิจกรรมตามพื้นฐาน

| กลุ่ม | แนวทาง |
|---|---|
| ห้อง ก | เน้น Grade Calculator แบบเงื่อนไขต่อเนื่องและ test case ขอบเขต |
| ห้อง ข | เพิ่ม validation เช่น คะแนนต้องอยู่ระหว่าง 0-100 และเพิ่ม Boolean Logic หลายเงื่อนไข |

## Output ช่วงเช้า

1. Flowgorithm Grade Calculator
2. Flowgorithm Exam Eligibility
3. Pseudocode
4. Truth Table
5. Test Case Table

---

# ช่วงบ่าย 13:00 - 16:00 น.  
## Flowgorithm Lab 3: Loop, Trace Table & Source Code Demo

## เป้าหมายช่วงบ่าย

1. เข้าใจแนวคิดการทำซ้ำหรือ Loop
2. ใช้ Counter และ Accumulator ได้
3. ไล่ค่าตัวแปรด้วย Trace Table ได้
4. ใช้ Flowgorithm สร้าง flowchart ที่มี loop ได้
5. เปิดดู Source Code จาก Flowgorithm ได้
6. อธิบายความสัมพันธ์ระหว่าง Flowchart และ Code ได้

## โครงสร้างเวลา

| เวลา | กิจกรรม |
|---:|---|
| 13:00 - 13:25 | Loop, Counter, Accumulator |
| 13:25 - 14:15 | Lab 5: Average Score |
| 14:15 - 14:40 | Trace Table |
| 14:40 - 14:55 | พัก |
| 14:55 - 15:25 | Source Code Viewer Demo |
| 15:25 - 15:50 | Mini Demo กลุ่มย่อย |
| 15:50 - 16:00 | Reflection Day 03 |

## Loop, Counter, Accumulator

- Loop คือการทำซ้ำ
- Counter คือตัวนับรอบ
- Accumulator คือตัวแปรสะสมค่า
- ต้องมีเงื่อนไขหยุด loop ไม่เช่นนั้นจะเกิด loop ไม่จบ

## Lab 5: Average Score

โจทย์

> รับคะแนนหลายวิชา แล้วคำนวณคะแนนเฉลี่ย

สำหรับห้อง ก: กำหนดจำนวนวิชาเป็น 3 หรือ 5 วิชา  
สำหรับห้อง ข: ให้ผู้ใช้กรอกจำนวนวิชาเอง

Logic พื้นฐาน

```text
total = 0
count = 1

WHILE count <= numberOfSubjects
    INPUT score
    total = total + score
    count = count + 1
ENDWHILE

average = total / numberOfSubjects
DISPLAY average
```

## Trace Table

ตัวอย่างคะแนน 3 วิชา: 10, 20, 30

| รอบ | score | total ก่อนบวก | total หลังบวก | count |
|---:|---:|---:|---:|---:|
| 1 | 10 | 0 | 10 | 1 |
| 2 | 20 | 10 | 30 | 2 |
| 3 | 30 | 30 | 60 | 3 |

## Source Code Viewer Demo

หลังจาก flowchart ทำงานได้ ให้นักศึกษาเปิดดู source code ที่ Flowgorithm สร้างขึ้น

ภาษาที่แนะนำให้ demo

- Python: อ่านง่าย เหมาะกับผู้เริ่มต้น
- JavaScript: เชื่อมโยงกับ Web Technology ได้ดี
- C/C++ หรือ Java: ใช้เปรียบเทียบถ้าหลักสูตรจะเรียนต่อในอนาคต

สิ่งที่ให้นักศึกษาสังเกต

| Flowgorithm | Code ที่เกี่ยวข้อง |
|---|---|
| Input | การรับค่าจากผู้ใช้ |
| Output | การแสดงผล |
| Assignment | การกำหนดค่าตัวแปร |
| If | คำสั่งเงื่อนไข |
| Loop | คำสั่งทำซ้ำ |

## Mini Demo

ให้แต่ละกลุ่มนำเสนอ 3 นาที

1. โจทย์ที่ทำคืออะไร
2. Input คืออะไร
3. Logic สำคัญคืออะไร
4. Flowchart ทำงานอย่างไร
5. ทดสอบด้วยข้อมูลอะไร
6. Source Code ที่ Flowgorithm แสดงมีหน้าตาอย่างไร
7. สิ่งที่เข้าใจเพิ่มขึ้นคืออะไร

## Output ช่วงบ่าย

1. Flowgorithm Average Score
2. Trace Table
3. Test Case Table
4. Source Code จาก Flowgorithm
5. Mini Demo

---

# Reflection Day 03

1. Loop ต่างจาก If อย่างไร
2. Counter และ Accumulator ใช้ทำอะไร
3. Trace Table ช่วยให้เข้าใจโปรแกรมอย่างไร
4. Source Code Viewer ทำให้เห็นภาพการเขียนโปรแกรมจริงอย่างไร
5. เรื่องใดที่ยังต้องฝึกเพิ่ม

---

# Output รวม Day 03

1. Flowgorithm Grade Calculator
2. Flowgorithm Exam Eligibility
3. Flowgorithm Average Score
4. Pseudocode
5. Truth Table
6. Test Case Table
7. Trace Table
8. Source Code จาก Flowgorithm
9. Mini Demo
10. Reflection Day 03
