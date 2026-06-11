# Day04 — ช่วงที่ 2: 11:00 - 12:00 น.
# Web Technology Landscape: เว็บปัจจุบันใช้เทคโนโลยีอะไร
## เอกสารเนื้อหาโดยละเอียดสำหรับกิจกรรมปรับพื้นฐานนักศึกษาใหม่
### วศ.บ. วิศวกรรมซอฟต์แวร์ ปีการศึกษา 2569

---

## 1. บทบาทของหัวข้อนี้ใน Day04

หัวข้อนี้อยู่ระหว่างช่วง **AI Literacy** และช่วง **Computer Network Fundamentals** จึงควรทำหน้าที่เป็น “สะพาน” ระหว่างโลก AI/Software ที่นักศึกษาเห็นในชีวิตประจำวัน กับพื้นฐานเครือข่ายที่ทำให้เว็บทำงานได้จริง

นักศึกษาใหม่อาจเคย “ใช้เว็บ” ทุกวัน แต่ยังไม่เห็นว่าเว็บไซต์หรือเว็บแอปสมัยใหม่ประกอบด้วยหลายส่วน เช่น

- Browser
- HTML / CSS / JavaScript
- Frontend framework
- Backend
- API
- Database
- Authentication
- Cloud / Server
- Deployment
- Security
- Performance
- Responsive design
- AI-enabled features

เป้าหมายของหัวข้อนี้ไม่ใช่สอนเขียนเว็บให้ครบภายใน 1 ชั่วโมง แต่ต้องทำให้นักศึกษาเห็น “แผนที่ของโลกเว็บ” ว่าแต่ละส่วนคืออะไร อยู่ตรงไหน และจะได้เรียนลึกขึ้นอย่างไรในหลักสูตรวิศวกรรมซอฟต์แวร์

---

## 2. เป้าหมายการเรียนรู้

หลังจบช่วง 1 ชั่วโมงนี้ นักศึกษาควรสามารถ

1. อธิบายภาพรวมการทำงานของเว็บไซต์หรือเว็บแอปได้
2. แยกส่วนประกอบหลักของระบบเว็บได้ ได้แก่ frontend, backend, API, database, server/cloud
3. เข้าใจบทบาทของ HTML, CSS, JavaScript และ TypeScript ในระดับเบื้องต้น
4. รู้จักตัวอย่าง framework และเครื่องมือที่ใช้ในงานเว็บปัจจุบัน
5. เข้าใจว่าเว็บสมัยใหม่ต้องคิดเรื่อง responsive design, performance, security และ accessibility
6. วิเคราะห์เว็บหรือแอปที่คุ้นเคยแบบ “Web Stack Detective” ได้
7. เชื่อมโยง Web Technology กับการเรียน Software Engineering ในปีที่ 1–4 ได้

---

## 3. โครงเวลา 1 ชั่วโมง

| เวลา | กิจกรรม | เป้าหมาย |
|---:|---|---|
| 11:00 - 11:05 | Hook: เมื่อกดเปิดเว็บ 1 หน้า เกิดอะไรขึ้นบ้าง | กระตุ้นความสนใจ |
| 11:05 - 11:12 | Web 101: Browser, URL, HTTP/HTTPS, HTML/CSS/JS | ปูพื้นภาพรวม |
| 11:12 - 11:25 | Frontend: สิ่งที่ผู้ใช้เห็นและโต้ตอบ | เข้าใจหน้าบ้านของเว็บ |
| 11:25 - 11:35 | Backend, API และ Database | เข้าใจหลังบ้านและข้อมูล |
| 11:35 - 11:45 | Modern Web Stack & Workflow | เห็นเทคโนโลยีปัจจุบัน |
| 11:45 - 11:55 | Activity: Web Stack Detective | ฝึกวิเคราะห์เว็บจริง |
| 11:55 - 12:00 | Wrap-up / Exit Ticket | สรุปและเชื่อมไป Network Fundamentals |

---

## 4. Big Picture: เว็บหนึ่งเว็บมีอะไรอยู่ข้างหลัง

ภาพรวมระบบเว็บอย่างง่าย

```text
User
  ↓
Browser / Mobile WebView
  ↓
Frontend: HTML + CSS + JavaScript
  ↓
API: REST / GraphQL / WebSocket
  ↓
Backend: Business Logic / Auth / Validation
  ↓
Database / File Storage / External Services
  ↓
Cloud / Server / CDN / Monitoring
```

| ส่วน | อธิบายแบบนักศึกษาใหม่ |
|---|---|
| User | คนที่ใช้งานเว็บ |
| Browser | โปรแกรมที่แสดงเว็บ เช่น Chrome, Edge, Safari, Firefox |
| Frontend | ส่วนที่ผู้ใช้เห็นและกดใช้งาน |
| Backend | ส่วนที่ประมวลผลเบื้องหลัง เช่น login, order, score |
| API | ช่องทางให้ frontend คุยกับ backend |
| Database | ที่เก็บข้อมูล เช่น user, product, score, order |
| Server / Cloud | ที่รันระบบและให้บริการผ่าน internet |
| CDN | ระบบกระจายไฟล์ static เช่น image, CSS, JS ให้โหลดเร็วขึ้น |
| Monitoring | ระบบดูสถานะว่าเว็บล่ม ช้า หรือ error หรือไม่ |

---

## 5. Hook: เมื่อกดเปิดเว็บ 1 หน้า เกิดอะไรขึ้นบ้าง?

### คำถามเปิด

> เมื่อเราเปิดเว็บ เช่น ระบบ LMS หรือเว็บร้านค้าออนไลน์ จากการพิมพ์ URL ไปจนเห็นหน้าเว็บ เกิดอะไรขึ้นบ้าง?

ให้นักศึกษาลองตอบก่อน 1–2 นาที แล้วค่อยเฉลยเป็นลำดับ

### เฉลยแนวคิดแบบเข้าใจง่าย

1. ผู้ใช้พิมพ์ URL หรือกด link
2. Browser ตรวจว่า URL คืออะไร
3. เครื่องต้องรู้ว่า domain นี้อยู่ที่ server ใด
4. Browser ส่ง request ผ่าน internet
5. Server ส่งไฟล์หรือข้อมูลกลับมา
6. Browser อ่าน HTML, CSS, JavaScript
7. หน้าเว็บแสดงผล
8. JavaScript อาจเรียก API เพิ่มเติม
9. API ติดต่อ backend และ database
10. ผู้ใช้เห็นข้อมูลล่าสุด เช่น รายวิชา คะแนน สินค้า หรือสถานะคำสั่งซื้อ

### ประเด็นสำคัญ

สิ่งที่ผู้ใช้เห็นคือ “หน้าเว็บ” แต่สิ่งที่ระบบทำจริงมีทั้ง browser, network, server, API, database และ security

---

## 6. Web 101: พื้นฐานเว็บที่ต้องรู้

### 6.1 URL

URL คือที่อยู่ของทรัพยากรบนเว็บ เช่น

```text
https://example.com/courses/intro-se?page=1#overview
```

| ส่วน | ตัวอย่าง | ความหมาย |
|---|---|---|
| Protocol | `https://` | วิธีสื่อสาร |
| Domain | `example.com` | ชื่อเว็บไซต์ |
| Path | `/courses/intro-se` | ตำแหน่งของหน้า/ข้อมูล |
| Query String | `?page=1` | ส่งค่าประกอบ request |
| Fragment | `#overview` | ชี้ตำแหน่งในหน้าเว็บ |

### 6.2 HTTP / HTTPS

HTTP คือ protocol ที่ browser ใช้คุยกับ server  
HTTPS คือ HTTP ที่เข้ารหัสเพื่อความปลอดภัย

ตัวอย่าง request/response แบบง่าย

```text
Browser: ขอหน้า /login
Server: ส่ง HTML/CSS/JS กลับมา

Browser: ส่ง username/password ไปตรวจสอบ
Server: ตอบว่า login สำเร็จหรือไม่
```

ข้อความที่ควรย้ำ

> เว็บไซต์สมัยใหม่ควรใช้ HTTPS เป็นมาตรฐาน โดยเฉพาะเว็บที่มี login, ข้อมูลส่วนตัว หรือข้อมูลธุรกรรม

### 6.3 Browser

Browser ไม่ใช่แค่โปรแกรมเปิดเว็บ แต่เป็น runtime สำหรับ web application

Browser ทำงานหลายอย่าง เช่น

- อ่าน HTML
- แสดงผล CSS
- รัน JavaScript
- ติดต่อ API
- จัดการ cookie / local storage
- ตรวจ security บางส่วน
- รองรับ responsive layout
- มี developer tools สำหรับนักพัฒนา

---

## 7. Frontend: สิ่งที่ผู้ใช้เห็นและโต้ตอบ

Frontend คือส่วนของเว็บที่ทำงานฝั่งผู้ใช้ เช่น หน้าเว็บ ปุ่ม ฟอร์ม เมนู ตาราง กราฟ dashboard และ interaction

### 7.1 HTML

HTML ใช้กำหนดโครงสร้างเนื้อหา เช่น heading, paragraph, link, image, form, table, button

```html
<h1>Welcome to SE Bootcamp</h1>
<p>เรียนรู้พื้นฐานเว็บและซอฟต์แวร์</p>
<button>เริ่มกิจกรรม</button>
```

### 7.2 CSS

CSS ใช้กำหนดรูปลักษณ์ เช่น สี ขนาด layout spacing typography responsive design และ animation

```css
button {
  background: teal;
  color: white;
  border-radius: 12px;
}
```

### 7.3 JavaScript

JavaScript ใช้ทำให้เว็บโต้ตอบได้ เช่น กดปุ่มแล้วเปลี่ยนข้อมูล ตรวจ form ก่อนส่ง เรียก API แสดงกราฟ และทำ single page application

```javascript
button.addEventListener("click", () => {
  alert("Hello Web!");
});
```

### 7.4 TypeScript

TypeScript คือ JavaScript ที่เพิ่มระบบ type ช่วยลดข้อผิดพลาดและทำให้ project ขนาดใหญ่ดูแลได้ง่ายขึ้น

```typescript
function calculateTotal(price: number, qty: number): number {
  return price * qty;
}
```

ประเด็นที่ควรสื่อ

> JavaScript ทำให้เว็บมีชีวิต ส่วน TypeScript ช่วยให้การพัฒนาเว็บขนาดใหญ่เป็นระบบมากขึ้น

---

## 8. Frontend Framework และ UI Ecosystem

เว็บปัจจุบันจำนวนมากไม่ได้เขียน HTML/CSS/JS ล้วนทั้งหมด แต่ใช้ framework หรือ library เพื่อช่วยจัดการ UI และ state

| เครื่องมือ | ภาพรวม |
|---|---|
| React | library ยอดนิยมสำหรับสร้าง UI แบบ component |
| Vue | framework ที่เรียนรู้ง่าย เหมาะกับ UI reactive |
| Angular | framework ขนาดใหญ่ มีโครงสร้างชัด |
| Svelte | compile-time framework เขียนสั้นและเร็ว |
| Solid | reactive UI library ที่เน้น performance |

### แนวคิด Component

Component คือชิ้นส่วน UI ที่นำกลับมาใช้ซ้ำได้ เช่น Button, Card, Navbar, Login Form, Product Item, Course Card, Score Table

```text
Page
 ├── Navbar
 ├── CourseList
 │    ├── CourseCard
 │    └── CourseCard
 └── Footer
```

### CSS Framework / UI Library ตัวอย่าง

| ประเภท | ตัวอย่าง |
|---|---|
| Utility CSS | Tailwind CSS |
| Component Framework | Bootstrap, Bulma |
| UI Component Library | MUI, Ant Design, shadcn/ui |
| Animation | CSS Animation, Framer Motion |

---

## 9. Backend: สิ่งที่ทำงานเบื้องหลัง

Backend คือส่วนที่ผู้ใช้มองไม่เห็นโดยตรง แต่ทำงานสำคัญ เช่น

- login / logout
- ตรวจสิทธิ์
- จัดการข้อมูล
- คำนวณ business rule
- เชื่อมต่อ database
- ส่ง email / notification
- เชื่อม payment / external service
- สร้าง report
- ตรวจ log และ error

### ภาษา Backend ตัวอย่าง

| ภาษา | ใช้กับอะไรได้บ้าง |
|---|---|
| JavaScript / TypeScript | Node.js, Express, NestJS |
| Python | FastAPI, Django, Flask |
| PHP | Laravel |
| Java | Spring Boot |
| C# | ASP.NET Core |
| Go | API service, cloud service |
| Ruby | Ruby on Rails |

### Backend Framework ตัวอย่าง

| Framework | ภาษา | จุดเด่นแบบสั้น |
|---|---|---|
| Express | JavaScript | เรียบง่าย ยืดหยุ่น |
| NestJS | TypeScript | โครงสร้างชัด เหมาะกับระบบใหญ่ |
| FastAPI | Python | สร้าง API ได้เร็ว เอกสาร API อัตโนมัติ |
| Django | Python | ครบเครื่องสำหรับ web application |
| Laravel | PHP | เหมาะกับ web application และระบบธุรกิจ |
| Spring Boot | Java | ใช้ใน enterprise system |
| ASP.NET Core | C# | ใช้ในองค์กรและระบบขนาดใหญ่ |

---

## 10. API: ช่องทางให้ระบบคุยกัน

API คือข้อตกลงหรือช่องทางให้ frontend หรือระบบอื่นคุยกับ backend

### ตัวอย่าง API

Frontend ขอข้อมูลรายวิชา

```text
GET /api/courses
```

Backend ตอบกลับเป็น JSON

```json
[
  {
    "id": 1,
    "name": "Introduction to Software Engineering",
    "credit": 3
  }
]
```

### REST API

| Method | ใช้ทำอะไร | ตัวอย่าง |
|---|---|---|
| GET | อ่านข้อมูล | GET /api/courses |
| POST | สร้างข้อมูล | POST /api/courses |
| PUT / PATCH | แก้ไขข้อมูล | PATCH /api/courses/1 |
| DELETE | ลบข้อมูล | DELETE /api/courses/1 |

### GraphQL

GraphQL เป็นอีกแนวทางหนึ่งที่ให้ client ระบุข้อมูลที่ต้องการได้ละเอียดขึ้น เหมาะกับบางระบบที่มีข้อมูลซับซ้อน

### WebSocket

WebSocket ใช้สำหรับการสื่อสารแบบ real-time เช่น chat, live notification, dashboard แบบ real-time, game และ live collaboration

---

## 11. Database และ Data Layer

Database คือที่เก็บข้อมูลของระบบ

### Database แบบ relational

เหมาะกับข้อมูลที่มีโครงสร้างชัด เช่น user, course, enrollment, order, payment

| Database | ใช้บ่อยในงาน |
|---|---|
| PostgreSQL | web app, enterprise, analytics |
| MySQL / MariaDB | web app, CMS, business system |
| SQL Server | ระบบองค์กร |
| SQLite | app ขนาดเล็กหรือ local development |

### Database แบบ NoSQL

| Database | ลักษณะ |
|---|---|
| MongoDB | document database |
| Redis | cache / key-value |
| Firebase Firestore | real-time / serverless app |
| DynamoDB | cloud-native NoSQL |

### สิ่งที่นักศึกษาควรเข้าใจ

- Frontend ไม่ควรเข้าถึง database โดยตรงในระบบจริงส่วนใหญ่
- Backend/API ทำหน้าที่ตรวจสอบและจัดการข้อมูลก่อนบันทึก
- Database ต้องคิดเรื่องความถูกต้อง ความปลอดภัย backup และ performance

---

## 12. Modern Web Architecture

### 12.1 Static Website

เหมาะกับเว็บเนื้อหา เช่น portfolio, landing page, documentation

```text
HTML/CSS/JS → CDN → Browser
```

### 12.2 Dynamic Web Application

เหมาะกับเว็บที่มี login และข้อมูลเปลี่ยนตามผู้ใช้

```text
Browser → Frontend → API → Backend → Database
```

### 12.3 Single Page Application (SPA)

โหลดหน้าเว็บหลักครั้งแรก แล้ว JavaScript จัดการการเปลี่ยนหน้าภายใน browser

ตัวอย่างแนวคิด: React app, Vue app, dashboard, admin panel

### 12.4 Server-Side Rendering (SSR)

Server สร้าง HTML ให้ก่อนส่งไปยัง browser ทำให้โหลดเร็วขึ้นในบางกรณีและเหมาะกับ SEO

ตัวอย่างเครื่องมือ: Next.js, Nuxt, SvelteKit

### 12.5 Static Site Generation (SSG)

สร้างไฟล์ HTML ล่วงหน้าตอน build เหมาะกับเว็บเนื้อหาที่ไม่เปลี่ยนบ่อย

### 12.6 Serverless / Edge

รัน function หรือ service บน cloud โดยไม่ต้องดูแล server เองโดยตรง เหมาะกับ API บางประเภท งาน event-driven หรือการ deploy ใกล้ผู้ใช้

---

## 13. Development Workflow สมัยใหม่

Workflow ทั่วไปของนักพัฒนาเว็บ

```text
Requirement
  ↓
Design UI / Wireframe
  ↓
Create Project
  ↓
Develop Frontend / Backend
  ↓
Connect API / Database
  ↓
Test
  ↓
Deploy
  ↓
Monitor & Improve
```

### เครื่องมือที่ควรรู้จัก

| กลุ่ม | ตัวอย่าง |
|---|---|
| Editor | VS Code |
| Version Control | Git, GitHub |
| Package Manager | npm, pnpm, yarn |
| Build Tool | Vite |
| API Testing | Postman, Insomnia, Thunder Client |
| Database Tool | pgAdmin, DBeaver, Prisma Studio |
| Deployment | Vercel, Netlify, Render, Railway, Cloudflare, Docker |
| Monitoring | log, metrics, error tracking |

### แนวคิดที่ควรสื่อ

- นักพัฒนาเว็บไม่ได้เขียนไฟล์ HTML แยก ๆ อย่างเดียว
- เว็บสมัยใหม่มี project structure, dependency, build, test และ deploy
- Git และ GitHub สำคัญมากสำหรับการทำงานเป็นทีม
- AI assistant อาจช่วยอธิบาย code หรือเสนอแนวทางได้ แต่ผู้เรียนต้องตรวจสอบเอง

---

## 14. Responsive Design, Accessibility และ Performance

### 14.1 Responsive Design

เว็บต้องใช้งานได้หลายขนาดหน้าจอ เช่น smartphone, tablet, notebook, desktop และ projector

แนวคิด

```text
Mobile-first → Tablet → Desktop
```

สิ่งที่ควรคิด

- ขนาดตัวอักษร
- spacing
- ปุ่มกดง่ายบนมือถือ
- รูปภาพไม่ล้นจอ
- ตารางควร scroll ได้บนจอเล็ก
- layout ควรเปลี่ยนตามขนาดหน้าจอ

### 14.2 Accessibility

Accessibility คือการทำให้คนหลากหลายกลุ่มเข้าถึงเว็บได้ เช่น คนสายตาไม่ดี คนใช้ keyboard navigation คนใช้ screen reader คนที่มีอุปกรณ์หรือ internet จำกัด และคนที่ใช้มือถือจอเล็ก

ตัวอย่างพื้นฐาน

- ใช้ heading ให้ถูก
- ปุ่มมีข้อความชัด
- สี contrast เพียงพอ
- รูปภาพมี alt text
- form มี label
- ใช้งานด้วย keyboard ได้

### 14.3 Performance

Performance คือความเร็วและความลื่นไหลของเว็บ

สิ่งที่ส่งผลต่อ performance

- ขนาดรูปภาพ
- จำนวน JavaScript
- ฟอนต์
- network
- server response
- cache
- database query
- third-party scripts

คำถามชวนคิด

> ถ้าเว็บสวยมากแต่โหลดช้า นักศึกษาคิดว่าผู้ใช้จะรู้สึกอย่างไร?

---

## 15. Web Security พื้นฐานที่ควรรู้ตั้งแต่ต้น

แม้เป็นช่วงปรับพื้นฐาน ก็สามารถย้ำแนวคิด security แบบง่ายได้

| ประเด็น | ตัวอย่าง |
|---|---|
| Authentication | login ต้องตรวจตัวตน |
| Authorization | ผู้ใช้แต่ละคนต้องมีสิทธิ์ต่างกัน |
| Input Validation | ตรวจข้อมูลที่ผู้ใช้กรอก |
| SQL Injection | ไม่ควรต่อ string query แบบเสี่ยง |
| XSS | ไม่ควรแสดงข้อมูลผู้ใช้โดยไม่ป้องกัน |
| CSRF | ระวัง request ปลอม |
| Secrets | ไม่ควรเอา API key หรือ password ไปใส่ใน frontend |
| HTTPS | ควรเข้ารหัสการสื่อสาร |
| Dependency Security | library ที่ใช้ต้องดูแล update |

ข้อความสำคัญ

> เว็บที่ “ทำงานได้” ยังไม่พอ ต้อง “ปลอดภัยพอสำหรับผู้ใช้จริง” ด้วย

---

## 16. AI อยู่ตรงไหนใน Web Technology

ควรแตะเพียงสั้น ๆ เพื่อไม่ซ้ำกับ AI Literacy

AI ในเว็บอาจอยู่ในรูปแบบ

- chatbot บนเว็บไซต์
- search ที่ฉลาดขึ้น
- recommendation
- image recognition
- code assistant สำหรับ developer
- content moderation
- analytics

ภาพรวม architecture

```text
Frontend
  ↓
Backend API
  ↓
AI Service / Model API
  ↓
Result
  ↓
Frontend Display
```

ข้อควรย้ำ

- อย่าส่งข้อมูลส่วนตัวหรือข้อมูลลับไปยัง AI โดยไม่จำเป็น
- คำตอบจาก AI ต้องตรวจสอบ
- AI เป็นส่วนหนึ่งของ software system ไม่ใช่สิ่งแยกจากระบบ

---

## 17. ตัวอย่าง Web Stack ของระบบใกล้ตัว

### 17.1 ระบบ LMS

| ส่วน | ตัวอย่าง |
|---|---|
| Frontend | หน้า course, assignment, grade |
| Backend | login, course management, assignment submission |
| Database | user, course, assignment, score |
| Storage | file งาน เอกสารประกอบ |
| API | ดึงข้อมูลรายวิชา ส่งงาน ดูคะแนน |
| Security | role: student, teacher, admin |

### 17.2 E-Commerce

| ส่วน | ตัวอย่าง |
|---|---|
| Frontend | product list, cart, checkout |
| Backend | order, payment, promotion |
| Database | product, user, order, payment |
| API | search product, create order |
| External Service | payment gateway, logistics |
| Security | payment security, fraud detection |

### 17.3 AI Chatbot Website

| ส่วน | ตัวอย่าง |
|---|---|
| Frontend | chat UI |
| Backend | session, rate limit, prompt handling |
| AI Service | model API |
| Database | chat history, user profile |
| Security | privacy, content filtering, access control |
| Monitoring | cost, error, latency |

---

## 18. คำถามแบบถามก่อน–เฉลยทีหลัง

### คำถามที่ 1

**ถาม:** เมื่อเปิดเว็บ 1 หน้า เกิดอะไรขึ้นบ้างตั้งแต่ browser ไปถึง server?

**เฉลยแนวคิด:** Browser ส่ง request ผ่าน internet ไปยัง server, server ส่ง HTML/CSS/JS หรือข้อมูลกลับมา, browser แสดงผล และอาจเรียก API เพิ่มเติมเพื่อดึงข้อมูลจาก backend/database

### คำถามที่ 2

**ถาม:** Frontend กับ Backend ต่างกันอย่างไร?

**เฉลยแนวคิด:** Frontend คือส่วนที่ผู้ใช้เห็นและโต้ตอบ เช่น UI ปุ่ม ฟอร์ม ส่วน Backend คือส่วนประมวลผลเบื้องหลัง เช่น login, business logic, database, security

### คำถามที่ 3

**ถาม:** API คืออะไร?

**เฉลยแนวคิด:** API คือช่องทางหรือข้อตกลงให้ frontend หรือระบบอื่นส่ง request ไปหา backend เพื่ออ่าน สร้าง แก้ไข หรือลบข้อมูล

### คำถามที่ 4

**ถาม:** ทำไม frontend ไม่ควรติดต่อ database โดยตรงในระบบจริงส่วนใหญ่?

**เฉลยแนวคิด:** เพราะเสี่ยงต่อความปลอดภัยและการควบคุมข้อมูล ควรให้ backend/API ตรวจสิทธิ์ ตรวจข้อมูล และบังคับ business rule ก่อนเข้าถึง database

### คำถามที่ 5

**ถาม:** ทำไมเว็บปัจจุบันต้อง responsive?

**เฉลยแนวคิด:** เพราะผู้ใช้เข้าจากหลายอุปกรณ์ โดยเฉพาะมือถือ เว็บจึงต้องปรับ layout และขนาดองค์ประกอบให้เหมาะกับหน้าจอที่ต่างกัน

### คำถามที่ 6

**ถาม:** ถ้าเว็บสวยแต่โหลดช้ามาก ถือว่าดีหรือไม่?

**เฉลยแนวคิด:** ไม่ดี เพราะ performance มีผลต่อ user experience, accessibility และเป้าหมายทางธุรกิจหรือการใช้งาน

### คำถามที่ 7

**ถาม:** ถ้าเอา API key ลับไปใส่ใน JavaScript ฝั่ง frontend จะเกิดอะไรขึ้น?

**เฉลยแนวคิด:** ผู้ใช้หรือผู้ไม่หวังดีอาจดู key ได้จาก browser ทำให้เกิดความเสี่ยงด้าน security และค่าใช้จ่าย

---

## 19. กิจกรรมในห้องเรียน

### กิจกรรมที่ 1: Web Stack Detective

**เวลา:** 8–10 นาที  
**รูปแบบ:** กลุ่ม 2–3 คน  
**อุปกรณ์:** smartphone หรือ notebook

ให้นักศึกษาเลือก 1 เว็บไซต์หรือเว็บแอปที่คุ้นเคย เช่น

- LMS / Google Classroom
- ระบบทะเบียน
- Shopee / Lazada
- YouTube
- Google Maps
- Mobile Banking web
- เว็บไซต์มหาวิทยาลัย
- AI chatbot website

แล้ววิเคราะห์ตาม worksheet

| คำถาม | คำตอบ |
|---|---|
| เว็บ/แอปที่เลือกคืออะไร | |
| ผู้ใช้คือใคร | |
| Frontend มีองค์ประกอบอะไรบ้าง | |
| Backend น่าจะทำอะไร | |
| Database ต้องเก็บข้อมูลอะไร | |
| API ที่น่าจะมีคืออะไร | |
| ต้องมี authentication หรือไม่ | |
| ข้อมูลใดเป็นข้อมูลสำคัญหรือข้อมูลส่วนตัว | |
| ถ้าเว็บช้า ผู้ใช้อาจรู้สึกอย่างไร | |
| ถ้าเว็บไม่ปลอดภัย จะเกิดความเสี่ยงอะไร | |

### กิจกรรมที่ 2: Draw the Web Stack

ให้แต่ละกลุ่มวาด diagram ง่าย ๆ

```text
User
  ↓
Browser / Mobile
  ↓
Frontend
  ↓
API
  ↓
Backend
  ↓
Database
```

จากนั้นให้เติมว่าในระบบที่เลือก แต่ละช่องคืออะไร

ตัวอย่าง LMS

```text
Student
  ↓
Browser
  ↓
Course Page / Assignment Page
  ↓
Assignment API / Grade API
  ↓
LMS Backend
  ↓
Course DB / File Storage
```

### กิจกรรมที่ 3: Web Feature Card Sorting

แจกหรือแสดงรายการ feature แล้วให้นักศึกษาจัดกลุ่มว่าอยู่ฝั่ง Frontend, Backend, Database หรือ External Service

| Feature | คำตอบที่คาดหวัง |
|---|---|
| ปุ่ม Login | Frontend |
| ตรวจรหัสผ่าน | Backend |
| ตารางคะแนน | Frontend + Database |
| บันทึกคะแนน | Backend + Database |
| ส่ง email แจ้งเตือน | Backend + External Service |
| เก็บไฟล์งาน | Storage |
| ตรวจสิทธิ์อาจารย์/นักศึกษา | Backend |
| ค้นหาสินค้า | Frontend + Backend + Database/Search Service |

### กิจกรรมที่ 4: 3-Minute Exit Ticket

ให้นักศึกษาตอบสั้น ๆ

1. วันนี้ฉันเข้าใจคำว่า frontend ว่าอย่างไร
2. วันนี้ฉันเข้าใจคำว่า backend ว่าอย่างไร
3. เว็บหรือแอปหนึ่งตัวที่ฉันอยากลองวิเคราะห์ต่อคืออะไร
4. เรื่องที่ยังไม่เข้าใจคืออะไร

---

## 20. Mini Demo ที่แนะนำสำหรับอาจารย์

หากมี internet และเวลาเพียงพอ สามารถ demo สั้น ๆ 3–5 นาที

### Demo 1: เปิด Developer Tools

1. เปิดเว็บไซต์ตัวอย่าง
2. กด Inspect
3. ดู Elements ว่า HTML คืออะไร
4. ดู Network ว่ามี request หลายรายการ
5. ชี้ให้เห็นไฟล์ `.html`, `.css`, `.js`, image, API

### Demo 2: Network Request

1. เปิด Developer Tools → Network
2. refresh หน้าเว็บ
3. ให้ดูว่า browser โหลดหลายไฟล์
4. อธิบายว่าเว็บไม่ได้เป็นไฟล์เดียว แต่มี resource จำนวนมาก
5. ถ้าเห็น request ที่เป็น API ให้ยกตัวอย่างว่า frontend กำลังขอข้อมูลจาก backend

### Demo 3: Responsive View

1. เปิด Developer Tools → Toggle device toolbar
2. สลับขนาด mobile/tablet/desktop
3. แสดงให้เห็นว่า layout เปลี่ยน
4. เชื่อมกับ mobile-first design

---

## 21. Pre-test / Post-test ตัวอย่าง

### ข้อ 1
Frontend คืออะไร

A. ส่วนที่ผู้ใช้เห็นและโต้ตอบ  
B. เครื่อง server เท่านั้น  
C. Database  
D. ระบบสำรองข้อมูล  

**เฉลย:** A

### ข้อ 2
Backend ทำหน้าที่ใด

A. แสดงสีของปุ่มเท่านั้น  
B. ประมวลผล logic, ตรวจสิทธิ์ และจัดการข้อมูลเบื้องหลัง  
C. แทน monitor  
D. แทน CSS  

**เฉลย:** B

### ข้อ 3
API ใช้ทำอะไร

A. ให้ frontend หรือระบบอื่นคุยกับ backend  
B. ใช้แทน keyboard  
C. ใช้แทน monitor  
D. ใช้แทนรูปภาพ  

**เฉลย:** A

### ข้อ 4
ภาษาใดเป็นพื้นฐานสำคัญของ frontend web

A. HTML, CSS, JavaScript  
B. SQL เท่านั้น  
C. C อย่างเดียว  
D. Assembly เท่านั้น  

**เฉลย:** A

### ข้อ 5
ข้อใดเป็น database

A. PostgreSQL  
B. CSS  
C. HTML  
D. Browser  

**เฉลย:** A

### ข้อ 6
Responsive design หมายถึงอะไร

A. เว็บที่เปลี่ยน layout ให้เหมาะกับอุปกรณ์และขนาดหน้าจอ  
B. เว็บที่ไม่มีรูปภาพ  
C. เว็บที่ใช้เฉพาะ desktop  
D. เว็บที่ไม่มี backend  

**เฉลย:** A

### ข้อ 7
สิ่งใดไม่ควรใส่ไว้ใน JavaScript ฝั่ง frontend แบบเปิดเผย

A. API key ลับหรือ password  
B. ข้อความหัวข้อเว็บ  
C. ปุ่มกด  
D. CSS class name  

**เฉลย:** A

### ข้อ 8
REST API มักใช้ method ใดสำหรับอ่านข้อมูล

A. GET  
B. POST  
C. DELETE  
D. PATCH  

**เฉลย:** A

### ข้อ 9
ถ้าเว็บโหลดช้า อาจเกี่ยวข้องกับข้อใด

A. รูปภาพใหญ่เกินไป  
B. JavaScript มากเกินไป  
C. server response ช้า  
D. ถูกทุกข้อ  

**เฉลย:** D

### ข้อ 10
เหตุใดนักศึกษา SE ต้องเข้าใจ Web Technology Landscape

A. เพื่อจำชื่อ framework ให้ได้ทั้งหมด  
B. เพื่อเห็นภาพว่าเว็บหนึ่งระบบมีหลายส่วนและแต่ละส่วนทำงานร่วมกันอย่างไร  
C. เพื่อไม่ต้องเรียน programming  
D. เพื่อใช้ browser ได้เท่านั้น  

**เฉลย:** B

---

## 22. Output ที่ควรได้จากช่วงนี้

หลังจบช่วง 11:00–12:00 นักศึกษาควรมี

1. ความเข้าใจภาพรวม web architecture
2. ความเข้าใจ frontend, backend, API, database
3. Web Stack Worksheet อย่างน้อย 1 ชุด
4. Diagram ง่าย ๆ ของระบบเว็บที่เลือก
5. คำตอบ Exit Ticket
6. ความพร้อมเชื่อมต่อเข้าสู่ช่วง Network Fundamentals ตอนบ่าย

---

## 23. สรุปท้ายบทสำหรับอาจารย์

ประโยคสรุปที่ควรพูดท้ายช่วง

> เว็บปัจจุบันไม่ใช่แค่หน้า HTML แต่เป็นระบบที่รวม frontend, backend, API, database, cloud, security และ performance เข้าด้วยกัน นักศึกษา Software Engineering ไม่จำเป็นต้องจำชื่อ framework ทั้งหมดในวันนี้ แต่ต้องเริ่มเห็นภาพว่าเว็บหนึ่งระบบประกอบด้วยอะไร และแต่ละส่วนมีหน้าที่อย่างไร

---

## 24. แหล่งอ้างอิงและคำแนะนำสำหรับผู้สอน

- MDN Web Docs — Learn Web Development / MDN Curriculum  
  https://developer.mozilla.org/en-US/docs/Learn_web_development  
  https://developer.mozilla.org/en-US/curriculum/

- MDN Web Performance  
  https://developer.mozilla.org/en-US/docs/Web/Performance

- web.dev — Responsive Web Design Basics  
  https://web.dev/articles/responsive-web-design-basics

- OWASP Top 10 Web Application Security Risks  
  https://owasp.org/www-project-top-ten/

- Vite Official Guide  
  https://vite.dev/guide/

- Next.js Documentation  
  https://nextjs.org/docs

- HTTP Archive Web Almanac  
  https://almanac.httparchive.org/
