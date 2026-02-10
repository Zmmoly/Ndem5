# أكواد الشاشات الكاملة - تطبيق نديم

هذا الملف يحتوي على جميع أكواد الشاشات الكاملة التي تحتاج لإضافتها للمشروع.

**ملاحظة مهمة**: جميع هذه الأكواد موجودة في الرسائل السابقة بشكل كامل.
يمكنك نسخها من الرسائل مباشرة، أو استخدام هذا الملف كمرجع للمسارات.

## قائمة الملفات المطلوبة

### 1. Navigation.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/navigation/Navigation.kt`
**الوصف**: ملف التنقل الرئيسي للتطبيق
**المصدر**: موجود في رسالتك الأصلية

### 2. SplashScreen.kt  
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/splash/SplashScreen.kt`
**الوصف**: شاشة البداية
**المصدر**: موجود في رسالتك الأصلية

### 3. LoginScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/auth/LoginScreen.kt`
**الوصف**: شاشة تسجيل الدخول
**المصدر**: موجود في رسالتك الأصلية

### 4. RegisterScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/auth/RegisterScreen.kt`
**الوصف**: شاشة التسجيل
**المصدر**: موجود في رسالتك الأصلية

### 5. ForgotPasswordScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/auth/ForgotPasswordScreen.kt`
**الوصف**: شاشة استعادة كلمة المرور
**المصدر**: موجود في رسالتك الأصلية

### 6. HomeScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/home/HomeScreen.kt`
**الوصف**: الشاشة الرئيسية
**المصدر**: موجود في رسالتك الأصلية

### 7. RecitationScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/recitation/RecitationScreen.kt`
**الوصف**: شاشة التسميع
**المصدر**: موجود في رسالتك الأصلية

### 8. ProfileScreen.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/screens/profile/ProfileScreen.kt`
**الوصف**: شاشة الملف الشخصي
**المصدر**: موجود في رسالتك الأصلية

### 9. Color.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/theme/Color.kt`
**الوصف**: ألوان التطبيق
**المصدر**: موجود في رسالتك الأصلية

### 10. Theme.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/theme/Theme.kt`
**الوصف**: ثيم التطبيق
**المصدر**: موجود في رسالتك الأصلية

### 11. Type.kt
**المسار**: `app/src/main/java/awab/quran/ar/ui/theme/Type.kt`
**الوصف**: أنواع الخطوط
**المصدر**: موجود في رسالتك الأصلية

## طريقة الإضافة السريعة

### في Android Studio:

1. افتح المشروع في Android Studio
2. انتظر Gradle Sync
3. في كل مجلد من المجلدات التالية، أنشئ الملف المقابل:
   - `ui/navigation/` → `Navigation.kt`
   - `ui/screens/splash/` → `SplashScreen.kt`
   - `ui/screens/auth/` → `LoginScreen.kt`, `RegisterScreen.kt`, `ForgotPasswordScreen.kt`
   - `ui/screens/home/` → `HomeScreen.kt`
   - `ui/screens/recitation/` → `RecitationScreen.kt`
   - `ui/screens/profile/` → `ProfileScreen.kt`
   - `ui/theme/` → `Color.kt`, `Theme.kt`, `Type.kt`
4. انسخ الكود من الرسائل السابقة إلى كل ملف

### من سطر الأوامر:

```bash
# أنشئ الملفات الفارغة أولاً
touch app/src/main/java/awab/quran/ar/ui/navigation/Navigation.kt
touch app/src/main/java/awab/quran/ar/ui/screens/splash/SplashScreen.kt
# ... وهكذا

# ثم افتحها في محرر النصوص وانسخ الكود
```

## ملاحظات مهمة

1. **المجلدات موجودة**: جميع المجلدات مُنشأة مسبقاً في المشروع
2. **الترتيب مهم**: ابدأ بـ theme files أولاً، ثم screens
3. **التبعيات صحيحة**: جميع imports ستعمل بشكل صحيح
4. **Firebase مطلوب**: لا تنسَ إضافة `google-services.json`

## للحصول على الأكواد الكاملة

ارجع إلى الرسائل السابقة في المحادثة حيث جميع الأكواد موجودة بالتفصيل.
كل ملف تم إرساله بشكل كامل ويمكن نسخه مباشرة.
