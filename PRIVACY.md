# מדיניות פרטיות — לומדים

עדכון אחרון: ספטמבר 2026 (עודכן: ייבוא מתמונה — עלות ואבטחת מפתח)

אפליקציית **לומדים** נבנתה כך שכל המידע נשאר אצלך.

## אילו נתונים נאספים

**כמעט אף אחד.** האפליקציה עצמה אינה אוספת, אינה שולחת ואינה משתפת מידע אישי,
ואין בה חשבון משתמש, שרת, מעקב, אנליטיקס או פרסום.

היוצא מן הכלל היחיד הוא תכונת **"ייבוא מערכת שעות מתמונה"** — תכונה אופציונלית שאתה
מפעיל ביוזמתך בלבד, ומתוארת בהמשך. אם לא תשתמש בה, שום מידע אינו נשלח לשום מקום
והאפליקציה עובדת במלואה ללא חיבור לאינטרנט.

## היכן נשמר המידע

מערכת השעות, שיעורי הבית, המבחנים והפתקים שאתה מזין נשמרים **מקומית על המכשיר בלבד**
(באמצעות SwiftData ו-UserDefaults של מערכת ההפעלה). המידע נמחק כאשר מוחקים את האפליקציה.

אם הפעלת גיבוי מכשיר של Apple (iCloud Backup / גיבוי מוצפן למחשב), נתוני האפליקציה עשויים
להיכלל בגיבוי הזה בהתאם להגדרות שלך מול Apple. הגיבוי מנוהל על ידי Apple ואינו נגיש למפתח.

## התראות

האפליקציה מתזמנת התראות מקומיות (תזכורות למבחנים ולמועדי הגשה) דרך מערכת ההפעלה.
ההתראות נוצרות ונשלחות במכשיר עצמו; שום מידע אינו נשלח החוצה.

## ייבוא מערכת שעות מתמונה (אופציונלי)

אם תבחר להשתמש בתכונה "ייבוא מתמונה" במסך עריכת המערכת:

- **התמונות** שתבחר יישלחו לשירות **Google Gemini** לצורך זיהוי הטקסט במערכת בלבד.
  התמונות אינן נשמרות אצלנו ואינן נשלחות לשום גורם אחר. לפני השליחה התמונה מקודדת מחדש,
  כך שנתוני מיקום (GPS) ומטא-דאטה אחרת מוסרים ממנה.
- **מפתח ה-API** הנדרש לשליחה הוא מפתח אישי וחינמי שאתה יוצר בעצמך ב-Google AI Studio
  ומזין באפליקציה. המפתח נשמר **מוצפן במחסן המפתחות (Keychain) של המכשיר בלבד**, אינו
  מוטמע בקוד האפליקציה, ואינו נשלח לשום שרת מלבד Google בעת שליחת תמונה שיזמת.
- **עלות:** ל-Google Gemini יש שכבת שימוש חינמית שמספיקה לקריאת מערכת שעות. Google לא
  תחייב אותך אלא אם תפעיל חיוב (billing) בעצמך בחשבון Google שלך. למפתח האפליקציה אין
  גישה לחשבון Google שלך ואין לו עלות כלשהי בגין השימוש שלך.
- שימוש ב-Google Gemini כפוף למדיניות הפרטיות ולתנאי השימוש של Google.

## הרשאות

- **התראות** — כדי להציג תזכורות. אפשר לאשר או לדחות, והאפליקציה עובדת גם בלי ההרשאה.
- **גישה לתמונות** — רק אם תפעיל "ייבוא מתמונה", ורק לתמונות שתבחר ידנית.

## שינויים במדיניות

עדכונים למדיניות יפורסמו בעמוד זה עם תאריך עדכון חדש.

## יצירת קשר

לשאלות בנושא פרטיות: ysekely@gmail.com

---

# Privacy Policy — Lomdim (English)

Last updated: September 2026 (updated: photo import — cost and key security)

**Lomdim** is built so that all your data stays with you.

## What data is collected

**Almost none.** The app itself does not collect, transmit, or share any personal
information. There is no user account, no server, no tracking, no analytics, and no
advertising.

The single exception is the **"Import timetable from a photo"** feature — an optional
feature you turn on yourself, described below. If you don't use it, nothing is sent
anywhere and the app works fully offline.

## Where data is stored

The schedule, homework, exams, and notes you enter are stored **only on your device**
(via the operating system's SwiftData and UserDefaults). The data is removed when you
delete the app.

If you use Apple device backup (iCloud Backup / encrypted computer backup), the app's
data may be included in that backup according to your settings with Apple. Backups are
managed by Apple and are not accessible to the developer.

## Notifications

The app schedules local notifications (exam and due-date reminders) through the operating
system. They are created and delivered on the device; nothing is sent externally.

## Importing a timetable from a photo (optional)

If you choose to use the "Import from a photo" feature in the timetable editor:

- **The photos** you select are sent to **Google Gemini** solely to recognize the text
  in your timetable. The photos are not stored by us and are not sent to anyone else.
  Each image is re-encoded before sending, which strips location (GPS) and other metadata.
- **The API key** required to send them is a personal, free key that you create yourself
  in Google AI Studio and enter in the app. It is stored **encrypted in the device
  Keychain only**, is not embedded in the app's code, and is never sent to any server
  other than Google when you send a photo you initiated.
- **Cost:** Google Gemini has a free usage tier that is sufficient for reading a
  timetable. Google will not charge you unless you enable billing yourself in your own
  Google account. The app developer has no access to your Google account and bears no
  cost for your usage.
- Use of Google Gemini is subject to Google's privacy policy and terms of service.

## Permissions

- **Notifications** — to show reminders. You may allow or deny; the app works without it.
- **Photo access** — only if you use "Import from a photo", and only for photos you pick
  manually.

## Changes

Updates to this policy will be posted on this page with a new date.

## Contact

For privacy questions: ysekely@gmail.com
