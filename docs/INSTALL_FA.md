# نصب و بازیابی
نسخهٔ OrcaSlicer را در About بررسی کنید و بستهٔ متناظر را استخراج کنید. نصب‌کنندهٔ این بسته‌ها برای نصب دسکتاپ ویندوز است. مسیر نصب Microsoft Store متفاوت است.

## نصب پیش‌فرض
پروژهٔ خود را ذخیره کنید و OrcaSlicer را ببندید. Install.cmd را اجرا کنید و درخواست دسترسی Administrator را تأیید کنید. سپس برنامه را با زبان English باز کنید و با نگه‌داشتن نشانگر روی تنظیمات، توضیحات فارسی را بررسی کنید.

## مسیر سفارشی
PowerShell را در پوشهٔ استخراج‌شده باز کنید و مسیر واقعی نصب را جایگزین کنید.
```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File ".\Install-PersianHelp.ps1" -InstallDir "D:\OrcaSlicer"
```

## بازیابی در نسخهٔ ۲.۵
Restore-Previous.cmd فایل زبان قبل از نصب را از پشتیبان برمی‌گرداند.
برای مسیر سفارشی از فرمان زیر استفاده کنید.
```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File ".\Install-PersianHelp.ps1" -InstallDir "D:\OrcaSlicer" -RestorePrevious
```

## بازیابی در نسخهٔ ۲.۴
Restore-English.cmd فایل انگلیسی اصلی همراه بسته را برمی‌گرداند. برای بازگرداندن ترجمهٔ نصب‌شدهٔ قبلی، از پشتیبان زمان‌دار before-fa استفاده کنید.
برای برگرداندن انگلیسی در مسیر سفارشی از فرمان زیر استفاده کنید.
```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File ".\Install-PersianHelp.ps1" -InstallDir "D:\OrcaSlicer" -RestoreEnglish
```

## بررسی نسخهٔ ۲.۵
Audit-Tooltips.cmd به Python 3 و اینترنت نیاز دارد و نصب پیش‌فرض را بررسی می‌کند. برای مسیر سفارشی، اسکریپت audit_tooltips_v25.py را با --mo و مسیر فایل OrcaSlicer.mo اجرا کنید. انتظار ممیزی ۸۰۴ راهنما، شامل ۸۰۲ فارسی و دو عنوان مشترک انگلیسی است.
فایل all_tooltips.tsv ترجمهٔ هر ۸۰۴ متن را برای مطالعه دارد.

## عیب‌یابی
اگر توضیح فارسی نمایش داده نمی‌شود، زبان English، نسخهٔ برنامه و مسیر نصب را بررسی کنید. برای لینک Wiki روی عنوان تنظیم کلیک کنید. لینک به سایت اصلی در کد برنامه تعیین می‌شود.
پس از ارتقای OrcaSlicer، نسخهٔ سازگار بسته را استفاده کنید و ممیزی را تکرار کنید.
