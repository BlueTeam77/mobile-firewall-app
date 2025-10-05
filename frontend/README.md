```markdown
# 📱 Mobile Firewall - Frontend

## 📌 نظرة عامة
هذا المستودع يحتوي على الجزء **Frontend (الواجهة الأمامية)** من مشروع تطبيق **جدار الحماية للهاتف** (Mobile Firewall).  
الواجهة مسؤولة عن:
- عرض الحالة الأمنية للهاتف بشكل بصري وواضح.  
- إظهار التنبيهات للمستخدم مع خيارات (حظر – تجاهل – تفاصيل).  
- توفير **لوحة تحكم (Dashboard)** تحتوي على قائمة التطبيقات المراقبة وسجل التهديدات.  
- التكامل مع **Backend** لعرض البيانات الحية والتقارير.  

---

## 📂 هيكلية المشروع
```

frontend/
│── src/                     # الكود الأساسي للواجهة
│   ├── screens/             # الشاشات الرئيسية (Splash, Dashboard, Alerts, Settings)
│   ├── components/          # المكونات القابلة لإعادة الاستخدام
│   ├── services/            # الربط مع Backend عبر API
│   ├── assets/              # الصور والأيقونات والستايلات
│   └── utils/               # دوال وأدوات مساعدة
│
│── tests/                   # ملفات الاختبار للـ UI
│── docs/                    # توثيق إضافي
│── package.json / build.gradle
│── README.md                # هذا الملف

````

---

## ⚙️ المتطلبات
- **Android Native (Java/Kotlin)** (المرحلة الأولى).  
- بيئة تطوير:  
  - Android Studio.  
  - JDK 11+.  
- تصميمات جاهزة عبر **Figma** (يتم توفيرها من قبل فريق التصميم).  

---

## 🚀 طريقة التشغيل (Development Setup)
1. استنسخ المستودع:
   ```bash
   git clone https://github.com/<team-org>/mobile-firewall-app.git
   cd mobile-firewall-app/frontend
````

2. افتح المشروع عبر **Android Studio**.
3. تأكد من تثبيت الحزم المطلوبة عبر **Gradle**.
4. شغل التطبيق على محاكي أو جهاز Android حقيقي لمعاينة الواجهة.

---

## 🖼️ الشاشات الأساسية

* **Splash Screen**: شاشة البداية.
* **Dashboard**: تعرض حالة الأمان العامة (Safe / Warning / Danger).
* **Alerts Screen**: قائمة التنبيهات والإجراءات المتخذة.
* **Apps List**: قائمة التطبيقات المراقبة وتصنيفها.
* **Settings**: إعدادات التطبيق.

---

## 🧪 الاختبار

لتشغيل الاختبارات:

```bash
./gradlew test
```

* التحقق من:

  * ظهور التنبيهات بشكل صحيح.
  * عرض البيانات القادمة من الـ Backend.
  * تجربة واجهة المستخدم وسلاسة التنقل بين الشاشات.

---

## 🤝 المساهمة

1. أنشئ فرع جديد باسمك أو باسم الميزة:

   ```bash
   git checkout -b feature/<feature-name>
   ```
2. ارفع التعديلات:

   ```bash
   git commit -m "Add: وصف قصير للتعديل"
   git push origin feature/<feature-name>
   ```
3. افتح **Pull Request** لمراجعة الكود والتصميم.

---

## 📜 الرخصة

هذا المشروع يستخدم [MIT License](LICENSE).

---

🎨 **مسؤول الـ Frontend Lead Developer:** بهاء الدين

```
