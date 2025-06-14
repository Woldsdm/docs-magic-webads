# تنظیمات Canvas برای تبلیغات

<div dir="rtl">
برای نمایش تبلیغات با WebView در پکیج Magic WebAds، باید یک **Canvas جداگانه** مخصوص تبلیغات بسازید.

---

## ✅ مراحل ساخت Canvas تبلیغات

1. از منوی **Hierarchy**، یک **UI Canvas** جدید اضافه کنید
2. **Canvas** را انتخاب کنید و در پنجره **Inspector**:

   * **Render Mode** را روی **Screen Space - Overlay** بگذارید
   * بخش **Canvas Scaler** را باز کنید و مقدار **UI Scale Mode** را روی **Scale With Screen Size** تنظیم کنید
   * گزینه **Match** را روی **Width Or Height** قرار دهید (مثلاً مقدار 0.5)
   * **Reference Resolution** را روی **640 x 360** تنظیم کنید

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