# 🧠 کامپوننت WebAdsManager

<div dir="rtl">

کامپوننت **WebAdsManager** یک Singleton ساده است که در هنگام اجرای بازی، سرویس‌های تبلیغاتی (ScriptableObjectهای نوع `Service`) را کلون کرده و در حافظه نگه می‌دارد. این کامپوننت مسئول مدیریت درخواست‌های تبلیغ و ارتباط با نمای تبلیغ (`UIAdView`) است.

---

## ✅ نحوه اضافه کردن WebAdsManager

برای اضافه کردن این کامپوننت:

1. یک **GameObject** در صحنه ایجاد کنید (مثلاً با نام `WebAds Manager`)
2. در **Inspector** روی گزینه `Add Component` کلیک کنید
3. به مسیر زیر بروید:

```
Magic WebAds > WebAds Manager
```

4. سرویس‌های تبلیغاتی که قبلاً ساختید (ScriptableObjectهای `Service`) رو به لیست `Services` در Inspector اضافه کنید


## 📸 تصویر کامپوننت WebAdsManager در اینسپکتور:

<p dir="rtl">
<img src="../Images/webadsmanager-inspector.png" alt="WebAdsManager Inspector">
</p>

---

## 🧩 وظایف کلیدی WebAdsManager

| وظیفه | توضیح |
|-------|-------|
| ذخیره Singleton | از طریق متغیر `Instance` قابل دسترسی است |
| کلون‌کردن سرویس‌ها | سرویس‌ها به صورت runtime کلون می‌شوند تا به آبجکت اصلی آسیبی وارد نشود |
| مدیریت درخواست‌ها | متد `GetAdRequests()` بر اساس فیلترهای نام تبلیغ، درخواست‌ها را برمی‌گرداند |
| مدیریت نمای تبلیغ | همه‌ی `UIAdView`ها را ثبت کرده و در زمان غیر فعال شدن، منابع آن‌ها را آزاد می‌کند |

---

## 🗂 متغیرهای Inspector

| نام متغیر | نوع | توضیحات |
|-----------|------|----------|
| `services` | `List<Service>` | لیستی از سرویس‌های تبلیغاتی تعریف‌شده که هنگام اجرا کلون می‌شوند |

---

## 🧩 ادامه‌ی آموزش:
📄 [مرحله بعد: تنظیمات Canvas](canvas-setup.md)

</div>