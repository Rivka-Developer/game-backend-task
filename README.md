# Game Management System - Backend Task

מערכת לניהול משחקים ומשתתפים המבוססת על Node.js ו-Prisma ORM.

## 🛠 טכנולוגיות
* **Runtime**: Node.js 18.
* **ORM**: Prisma.
* **Database**: PostgreSQL 15.
* **Infrastructure**: Docker & Docker Compose.

## 🚀 הרצה מהירה
כדי להקים את מסד הנתונים ולהריץ את האפליקציה, יש להריץ:
`docker-compose up --build`
הפקודה מבצעת אוטומטית: הרמת DB, סנכרון סכימה (db push) והרצת main.js.

## 📋 עיקרי המערכת
* **Schema**: מודל נתונים הכולל משתמשים, משחקים וטבלת קישור למשתתפים (Many-to-Many).
* **Business Logic**: שירות `joinGame` המבצע בדיקות תקינות על סטטוס המשחק ומניעת כפל רישום.
* **Auto-Seed**: המערכת מייצרת נתוני בדיקה ראשוניים (User & Game) עם ההפעלה.

---
*הערה: הוגדרו מעקפי SSL ב-Dockerfile ובהרצה לצורך תאימות בסביבות מסוננות.*
