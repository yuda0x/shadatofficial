# FIFA FHD Live — TahMiDx

## 📁 ফাইল স্ট্রাকচার
```
fifa-site/
├── index.html     ← মূল সাইট
├── vercel.json    ← Vercel কনফিগ
└── README.md
```

---

## 🚀 GitHub → Vercel Deploy গাইড

### Step 1 — GitHub Repository তৈরি করো
1. [github.com](https://github.com) → **New repository**
2. Repository name: `fifa-live` (বা যেকোনো নাম)
3. **Public** রাখো → **Create repository**

### Step 2 — ফাইল আপলোড করো
```
index.html   ← আপলোড করো
vercel.json  ← আপলোড করো
```
অথবা Git দিয়ে:
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/তোমার-username/fifa-live.git
git push -u origin main
```

### Step 3 — Vercel-এ Deploy করো
1. [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. **Add New Project** → তোমার `fifa-live` repo সিলেক্ট করো
3. Framework: **Other** রাখো
4. **Deploy** চাপো ✅

### Step 4 — সাইট Live! 🎉
Vercel তোমাকে একটা URL দেবে যেমন:
`https://fifa-live-username.vercel.app`

---

## ⚙️ কাস্টমাইজ করতে চাইলে

`index.html` এর `CONFIG` অবজেক্ট এডিট করো:

```js
const CONFIG = {
    fbPageUrl  : 'https://www.facebook.com/তোমার-পেজ',  // FB পেজ লিঙ্ক
    baseViews  : 6366,    // শুরুতে যত viewer দেখাবে
    lockerKey  : 'fifa_unlocked_v1',  // পরিবর্তন করলে locker রিসেট হবে
};
```

---

## 📺 Stream URL পরিবর্তন
Server বাটনগুলোর `onclick` এ নতুন URL বসাও।
