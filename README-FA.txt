سامانه مدیریت کتابخانه مدارس — بسته آماده GitHub Pages

محتویات:
- index.html: فایل اصلی برنامه (نسخه 1.5.0-saas)
- manifest.webmanifest: تنظیمات نصب‌پذیری PWA
- sw.js: سرویس‌ورکر و کش پوسته برنامه
- icon-192.png و icon-512.png و apple-touch-icon.png: آیکون‌ها

روش انتشار:
1) همه فایل‌های داخل این پوشه را در ریشه مخزن ketabkhaneh-madrese بارگذاری کنید.
2) در GitHub وارد Settings > Pages شوید.
3) در بخش Build and deployment، گزینه Deploy from a branch را انتخاب کنید.
4) Branch را main و پوشه را /(root) قرار دهید و Save را بزنید.
5) پس از پایان Deploy، نشانی زیر را باز کنید:
   https://amirhoseinabed667-cmd.github.io/ketabkhaneh-madrese/

نکته امنیتی:
کلید sb_publishable داخل index.html کلید عمومی کلاینت است و به‌تنهایی مجوز دسترسی امن ایجاد نمی‌کند؛ امنیت واقعی داده‌ها باید با RLS در Supabase اعمال شود. هرگز service_role key را در فایل‌های عمومی قرار ندهید.

محدودیت آفلاین:
این بسته پوسته صفحه را کش می‌کند، اما ورود، داده‌های ابری، اسکن آنلاین و کتابخانه‌های CDN برای کارکرد کامل به اینترنت نیاز دارند. این بسته به‌تنهایی تنظیمات دیتابیس یا سیاست‌های امنیتی Supabase را تغییر نمی‌دهد.
