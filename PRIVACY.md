# מדיניות פרטיות — לומדים

עדכון אחרון: ספטמבר 2026 (עודכן: יצירת כרטיסיות עם AI ומד שימוש)

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

האפליקציה מתזמנת התראות מקומיות (תזכורות למבחנים ולמועדי הגשה, ושאלה בערב שלפני הגשה אם
שיעורי הבית בוצעו) דרך מערכת ההפעלה. ההתראות נוצרות ונשלחות במכשיר עצמו; שום מידע אינו נשלח החוצה.

## מסך הנעילה והווידג'ט

הפעילות החיה (Live Activity) והווידג'ט מציגים את השיעור הנוכחי והבא על מסך הנעילה ומסך הבית.
המידע נקרא ממערכת השעות שלכם במכשיר בלבד. שימו לב: מה שמופיע על מסך הנעילה גלוי לכל מי
שמחזיק בטלפון; אפשר לכבות את הפעילות החיה במסך "אודות".

## תכונות AI: ייבוא מערכת מתמונה ויצירת כרטיסיות (אופציונלי)

שתי תכונות באפליקציה משתמשות ב-**Google Gemini**, ושתיהן אופציונליות ופועלות רק ביוזמתך:

- **ייבוא מתמונה:** **התמונות** שתבחר יישלחו ל-Gemini לצורך זיהוי הטקסט במערכת בלבד.
  התמונות אינן נשמרות אצלנו ואינן נשלחות לשום גורם אחר. לפני השליחה התמונה מקודדת מחדש,
  כך שנתוני מיקום (GPS) ומטא-דאטה אחרת מוסרים ממנה.
- **יצירת כרטיסיות עם AI:** כשתבקש זאת, **הטקסט** של הערת שיעור או של "מה צריך ללמוד"
  במבחן נשלח ל-Gemini יחד עם שם המקצוע, כדי לנסח שאלות ותשובות. לא נשלח שום דבר אחר —
  לא המערכת, לא שיעורי הבית, לא הציונים. אתה מאשר כל כרטיסייה לפני שהיא נשמרת.
- **הגבלה עצמית:** האפליקציה מגבילה את עצמה ל-20 פעולות AI ביום ומציגה במסך "אודות"
  כמה פעולות וכמה טוקנים נשלחו, לפי הספירה של Google.
- **מפתח ה-API** הנדרש לשליחה הוא מפתח אישי וחינמי שאתה יוצר בעצמך ב-Google AI Studio
  ומזין באפליקציה. המפתח נשמר **מוצפן במחסן המפתחות (Keychain) של המכשיר בלבד**, אינו
  מוטמע בקוד האפליקציה, ואינו נשלח לשום שרת מלבד Google בעת פעולה שיזמת.
- **עלות:** ל-Google Gemini יש שכבת שימוש חינמית שמספיקה לקריאת מערכת שעות. Google לא
  תחייב אותך אלא אם תפעיל חיוב (billing) בעצמך בחשבון Google שלך. למפתח האפליקציה אין
  גישה לחשבון Google שלך ואין לו עלות כלשהי בגין השימוש שלך.
- **הסכמה:** לפני השליחה הראשונה האפליקציה מציגה מסך הסבר ומבקשת הסכמה מפורשת. אפשר לבטל בכל רגע.
- **שכבה חינמית:** לפי תנאי Google, תוכן שנשלח דרך השכבה החינמית של Gemini API עשוי לשמש
  את Google לשיפור המוצרים שלה, וייתכן שייבדק על ידי בני אדם. זו הסיבה שהאפליקציה שולחת
  רק מה שבחרתם — תמונות או טקסט — ורק אחרי שאישרתם.
- שימוש ב-Google Gemini כפוף למדיניות הפרטיות ולתנאי השימוש של Google.

## הוספה ליומן (אופציונלי)

אם תבחרו להוסיף מבחן או מועד הגשה ליומן:

- **יומן אפל** — האפליקציה מבקשת הרשאת **כתיבה בלבד** ויוצרת אירוע אחד במכשיר.
  היא אינה קוראת את היומן שלכם, אינה מסנכרנת ממנו ואינה רואה אירועים אחרים.
- **Google Calendar** — נפתח קישור "יצירת אירוע" ממולא מראש בדפדפן או באפליקציה של Google.
  אין התחברות לחשבון Google מתוך האפליקציה, ולא נשמרים אסימוני גישה כלשהם.

הייצוא חד־כיווני בלבד, ונעשה רק בלחיצה יזומה שלכם.

## הרשאות

- **התראות** — כדי להציג תזכורות. אפשר לאשר או לדחות, והאפליקציה עובדת גם בלי ההרשאה.
- **גישה לתמונות** — רק אם תפעיל "ייבוא מתמונה", ורק לתמונות שתבחר ידנית.

## שינויים במדיניות

עדכונים למדיניות יפורסמו בעמוד זה עם תאריך עדכון חדש.

## יצירת קשר

לשאלות בנושא פרטיות: ysekely@gmail.com

---

# Privacy Policy — Lomdim (English)

Last updated: September 2026 (updated: AI flashcards and usage meter)

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

The app schedules local notifications (exam and due-date reminders, and a question the evening
before homework is due asking whether it's done) through the operating system. They are created
and delivered on the device; nothing is sent externally.

## Lock screen and widget

The Live Activity and the widget show the current and next class on the lock screen and home
screen. The information is read from your timetable on the device only. Note that whatever
appears on the lock screen is visible to anyone holding the phone; the Live Activity can be
turned off in the About screen.

## AI features: timetable import and flashcard generation (optional)

Two features use **Google Gemini**; both are optional and run only when you ask:

- **Import from a photo:** **the photos** you select are sent to Gemini solely to recognize
  the text in your timetable. The photos are not stored by us and are not sent to anyone
  else. Each image is re-encoded before sending, which strips location (GPS) and other metadata.
- **Create flashcards with AI:** when you ask for it, **the text** of a class note or of an
  exam's "what to study" is sent to Gemini together with the subject name, to draft questions
  and answers. Nothing else is sent — not your timetable, homework or grades. You approve
  every card before it is saved.
- **Self-imposed limit:** the app caps itself at 20 AI actions a day and shows in "About"
  how many actions and tokens were sent, as counted by Google.
- **The API key** required to send them is a personal, free key that you create yourself
  in Google AI Studio and enter in the app. It is stored **encrypted in the device
  Keychain only**, is not embedded in the app's code, and is never sent to any server
  other than Google for an action you initiated.
- **Cost:** Google Gemini has a free usage tier that is sufficient for reading a
  timetable. Google will not charge you unless you enable billing yourself in your own
  Google account. The app developer has no access to your Google account and bears no
  cost for your usage.
- **Consent:** before the first upload the app shows an explanation screen and asks for your
  explicit permission. You can cancel at any time.
- **Free tier:** under Google's terms, content sent through the free tier of the Gemini API may
  be used by Google to improve its products, and may be reviewed by humans. That is why the app
  sends only what you chose — photos or text — and only after you agreed.
- Use of Google Gemini is subject to Google's privacy policy and terms of service.

## Adding to your calendar (optional)

If you choose to add an exam or a due date to your calendar:

- **Apple Calendar** — the app requests **write-only** access and creates a single event on
  your device. It never reads your calendar, never syncs from it, and cannot see other events.
- **Google Calendar** — a pre-filled "create event" link opens in your browser or the Google
  Calendar app. There is no Google sign-in inside the app and no access tokens are stored.

The export is one-way only, and happens only when you tap it.

## Permissions

- **Notifications** — to show reminders. You may allow or deny; the app works without it.
- **Photo access** — only if you use "Import from a photo", and only for photos you pick
  manually.

## Changes

Updates to this policy will be posted on this page with a new date.

## Contact

For privacy questions: ysekely@gmail.com
