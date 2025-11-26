בס"ד
API  - תורים לטיפת חלב

🌼 נושא הפרויקט
מערכת לניהול תורים לתחנת טיפת חלב
________________________________________
🌼 תיאור הפרויקט
מערכת Back Office שמיועדת לצוות טיפת חלב ומאפשרת:
•	רישום תינוקות ומעקב אחרי סטטוס שלהם
•	ניהול צוות אחיות עם סטטוס (פעילה / בחל״ת / לא זמינה)
•	קביעת תורים לתינוקות
•	מחיקה אמיתית של תורים (DELETE)
•	שליפות חכמות של תורים לפי תאריך / אחות / סטטוס
________________________________________
🌼 ישויות במערכת
1.	Baby – תינוק
2.	Nurse – אחות
3.	Appointment – תור
🌼 מיפוי Routes
1️⃣ Baby (תינוק)
•	שליפת רשימת תינוקות:
GET https://tipa.co.il/babies
•	שליפת תינוק לפי מזהה:
GET https://tipa.co.il/babies/{id}
•	הוספת תינוק:
POST https://tipa.co.il/babies
•	עדכון תינוק:
PUT https://tipa.co.il/babies/{id}
•	❌ מחיקה לא קיימת
•	עדכון סטטוס תינוק (פעיל / לא פעיל / הועבר תחנה):
PUT https://tipa.co.il/babies/{id}/status
________________________________________
2️⃣ Nurse (אחות)
•	שליפת רשימת אחיות:
GET https://tipa.co.il/nurses
•	שליפת אחות לפי מזהה:
GET https://tipa.co.il/nurses/{id}
•	הוספת אחות:
POST https://tipa.co.il/nurses
•	עדכון אחות:
PUT https://tipa.co.il/nurses/{id}
•	❌ מחיקה לא קיימת
•	עדכון סטטוס אחות (פעילה / בחל״ת / לא זמינה):
PUT https://tipa.co.il/nurses/{id}/status
________________________________________
3️⃣ Appointment (תור)
•	שליפת רשימת תורים:
GET https://tipa.co.il/appointments
•	שליפת תור לפי מזהה:
GET https://tipa.co.il/appointments/{id}
•	הוספת תור:
POST https://tipa.co.il/appointments
•	עדכון תור:
PUT https://tipa.co.il/appointments/{id}
•	מחיקת תור:
DELETE https://tipa.co.il/appointments/{id}
•	שליפת תורים לפי תאריך:
GET https://tipa.co.il/appointments?date=2025-01-12



