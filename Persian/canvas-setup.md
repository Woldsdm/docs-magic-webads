# تنظیمات Canvas برای تبلیغات

<div dir="rtl">

برای نمایش تبلیغات با WebView در پکیج Magic WebAds، باید یک **Canvas جداگانه** مخصوص تبلیغات بسازید.

---

## ✅ مراحل ساخت Canvas تبلیغات

1. ابتدا از منوی **Hierarchy**، یک **UI Canvas** جدید اضافه کنید
2. سپس **Canvas** را انتخاب کنید و در پنجره **Inspector**:

* ابتدا گزینه **Render Mode** را روی **Screen Space - Overlay** بگذارید
* سپس بخش **Canvas Scaler** را باز کنید و مقدار **UI Scale Mode** را روی **Scale With Screen Size** تنظیم کنید
* همچنین گزینه **Match** را روی **Width Or Height** قرار دهید (مثلاً مقدار 0.5)
* در نهایت **Reference Resolution** را روی **640x360** تنظیم کنید

> ⚠️ این تنظیمات و ابعاد خیلی مهم هستند تا نمایش WebView روی اندروید با پیکسل‌های HTML و CSS همخوانی کامل داشته باشد.

---

## 🖼 تصویر Inspector Canvas

<p dir="rtl">
<img src="../Images/canvas-setup-inspector.png" alt="Canvas Setup Inspector">
</p>

---

## 🧩 ادامه‌ی آموزش:

📄 [مرحله‌ی بعد: کامپوننت UIAdView](uiadview.md)
</div>