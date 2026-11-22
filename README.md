# 🎙️ Transcription

**Transcription** تطبيق ويب (PWA) يحوّل الكلام العربي إلى كتابة صوتية IPA للهجات الأردنية (مدنية، ريفية، بدوية).

## الحالة
نموذج أولي: محرّك قواعد صوتية + معجم صغير. نموذج الصوت المباشر (audio → IPA) قيد التطوير.

## النشر على GitHub Pages
1. أنشئ مستودعاً جديداً على GitHub وارفع كل الملفات (بما فيها مجلد `.github`).
2. من Settings ← Pages ← Source اختر **GitHub Actions**.
3. أي push على فرع `main` ينشر التطبيق تلقائياً على:
   `https://USERNAME.github.io/REPO/`

## التثبيت كتطبيق
افتح الرابط من الموبايل (Chrome أو Safari) ← "إضافة إلى الشاشة الرئيسية".

## الملفات
- `index.html` التطبيق كاملاً
- `manifest.webmanifest` و `icon.svg` إعدادات التثبيت
- `sw.js` يخلّيه يشتغل بدون إنترنت
- `.github/workflows/pages.yml` النشر التلقائي

## تطوير المعجم
أضف كلمات جديدة في الكائن `LEX` داخل `index.html`. الرموز: `Q`=ق، `K`=ك، `J`=ج، والباقي IPA مباشرة.

## ملاحظة
التسجيل الصوتي يعتمد على Web Speech API ويتطلب HTTPS (GitHub Pages يوفّره).
