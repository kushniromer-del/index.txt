# 🧠 BrainFuzz

> משחק ויראלי מבוסס בלבול מוחי + תגובה מהירה + תחרות

[![Deploy](https://img.shields.io/badge/Live-GitHub%20Pages-brightgreen)]()

## 🎮 מה יש במשחק

| מצב | תיאור |
|-----|--------|
| ⚡ Solo Mode | שאלות מהירות, חוקים משתנים, 3 רמות קושי |
| 👥 מצב חברים | 2 שחקנים באותו מכשיר — מי ינצח? |
| 🏆 לידרבורד | שיאים לפי קטגוריה, עם מדינות |
| 🐱 לחץ / אל תלחץ | מיני גיים — החוק משתנה כל שנייה |
| 🧩 זיכרון מהיר | זכור אובייקטים ובחר אותם |
| 🎯 מצא חריג | מה לא שייך? — מהר! |

## 🚀 העלאה ל-GitHub Pages (5 דקות)

### שלב 1 — צור ריפו חדש
1. כנס ל-[github.com](https://github.com) → **New repository**
2. שם: `brainfuzz` (או כל שם אחר)
3. Public ✅ → **Create repository**

### שלב 2 — העלה את הקובץ
1. לחץ **Add file** → **Upload files**
2. גרור את `brainfuzz.html` לתוך הדף
3. שנה את שם הקובץ ל-`index.html` לפני ההעלאה (או עשה זאת מאוחר יותר)
4. לחץ **Commit changes**

### שלב 3 — הפעל GitHub Pages
1. כנס ל-**Settings** של הריפו
2. צד שמאל → **Pages**
3. תחת Source בחר: **Deploy from a branch**
4. Branch: **main** → folder: **/ (root)**
5. לחץ **Save**

### שלב 4 — קבל את הקישור!
אחרי כ-2 דקות הכתובת תהיה:
```
https://USERNAME.github.io/brainfuzz/
```

## 🌐 דרכים נוספות להפצה מהירה

### Netlify (הכי מהיר!)
1. כנס ל-[netlify.com](https://netlify.com) → **Add new site**
2. **Deploy manually** → גרור את `index.html`
3. מיד מקבל קישור ציבורי!

### Vercel
```bash
npx vercel --name brainfuzz
```

## 📱 תאימות
- ✅ נייד (iOS + Android)
- ✅ טאבלט
- ✅ מחשב (Chrome, Firefox, Safari, Edge)

## 🔧 התאמה אישית

פתח את `index.html` בעורך טקסט:

**שנה צבעים** — חפש `:root {` בתחילת ה-CSS
```css
--yellow: #FFE600;   /* צבע ראשי */
--pink:   #FF2D78;   /* אקסנט */
--cyan:   #00F5FF;   /* צבע משני */
```

**הוסף שאלות** — חפש `const QB = {` בסקריפט:
```js
math: [
  {q:'כמה זה X?', opts:['A','B','C','D'], a: 0}, // a = אינדקס התשובה הנכונה
  ...
]
```

**שנה קושי** — חפש `const times`:
```js
const times = {easy:15, medium:10, hard:6}; // שניות לשאלה
```

## 📊 מה שמור בלידרבורד

המשחק שומר שיאים ב-`localStorage` של הדפדפן.
בשלב 2 (לידרבורד אמיתי) אפשר לחבר Supabase / Firebase.

## 🛣️ רודמאפ

- [x] Solo Mode עם חוקים משתנים
- [x] Multiplayer (אותו מכשיר)  
- [x] לידרבורד מקומי
- [x] 3 מיני גיימס
- [ ] לידרבורד גלובלי (Firebase)
- [ ] שיתוף תוצאות כתמונה
- [ ] מצב ריצה מוגבלת בזמן
- [ ] PWA (התקנה כאפליקציה)

---

Built with ❤️ — BrainFuzz v1.0
