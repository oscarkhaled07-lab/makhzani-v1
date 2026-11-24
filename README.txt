مخزني - مراجعة المشروع وطريقة البناء

حالة المشروع:
- تطبيق Android أصلي باستخدام Kotlin و Jetpack Compose.
- تخزين البيانات محلياً على الهاتف باستخدام Room/SQLite.
- لا يحتاج إلى اتصال بالإنترنت أثناء الاستخدام.
- تم تحسين التحقق من الكميات والأسعار، ومنع القيم غير المحدودة، وإضافة معالجة للأخطاء عند حفظ المنتج والوصل.

فتح المشروع:
1) افتح مجلد Makhzani في Android Studio (يفضل إصدار حديث).
2) تأكد من تثبيت Android SDK 34 و JDK 17.
3) المشروع يحدد Gradle 8.7 و Android Gradle Plugin 8.5.2.
4) ملف gradle-wrapper.jar وسكربتا gradlew و gradlew.bat غير مرفقة في النسخة المستلمة. إذا لم يقم Android Studio بإنشاء/توفير Gradle Wrapper تلقائياً، أنشئه من طرفية Android Studio بعد توفر Gradle 8.7 بالأمر:
   gradle wrapper --gradle-version 8.7

إنشاء APK من Android Studio:
Build > Build Bundle(s) / APK(s) > Build APK(s)

أو بعد إنشاء Gradle Wrapper:
Windows: gradlew.bat assembleDebug
Linux/macOS: ./gradlew assembleDebug

مكان APK التجريبي:
app/build/outputs/apk/debug/app-debug.apk

ملاحظة التوقيع:
إعداد release الحالي يستخدم مفتاح debug للاستخدام الشخصي والتجربة فقط. قبل النشر العام يجب إعداد مفتاح توقيع خاص وعدم مشاركة ملفه أو كلمة مروره.
