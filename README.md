# Phantom Tunnel 👻

**ناپدید شوید. یک تونل قدرتمند و پنهان‌کار که راه‌اندازی آن به سادگی آب خوردن است.**

**فانتوم** پیچیدگی‌های ساخت تونل را از بین می‌برد. با یک منوی تعاملی و هوشمند، شما بدون نیاز به هیچ دانش فنی و تنها با پاسخ به چند سوال ساده، می‌توانید یک تونل امن، نامرئی و پایدار راه‌اندازی کنید.

## چرا فانتوم؟

-   **👻 راه‌اندازی فوق‌العاده آسان:** دیگر نیازی به فایل‌های کانفیگ یا دستورات پیچیده نیست. فقط برنامه را اجرا کنید و به سوالات پاسخ دهید.
-   **🔒 تولید خودکار SSL:** فانتوم به طور خودکار گواهی امنیتی (SSL) مورد نیاز سرور را تولید می‌کند. دیگر با دستورات `openssl` خداحافظی کنید.
-   **🤫 پنهان‌کاری مطلق:** مانند نسخه‌های قبلی، تمام ترافیک درون یک اتصال امن WebSocket (WSS) پنهان می‌شود و از دید سیستم‌های فیلترینگ نامرئی می‌ماند.
-   **⚡ عملکرد و پایداری بالا:** از همان معماری قدرتمند مبتنی بر مالتی‌پلکسینگ برای تضمین سرعت و پایداری اتصال استفاده می‌کند.

---

## نصب: فقط یک دستور تا نامرئی شدن

این دستور را در ترمینال لینوکس خود اجرا کنید. اسکریپت بقیه کارها را انجام می‌دهد.


```bash
bash <(curl -sSL https://raw.githubusercontent.com/webwizards-team/phantom-tunnel/main/install.sh)
```
> اسکریپت برای فعال ماندن بعد از بسته شدن ترمینال نیاز به دستور `tmux` خواهد داشت.

---

## نحوه استفاده

پس از نصب، کافیست دستور `phantom-tunnel` را در ترمینال خود وارد کنید.

### ۱. راه‌اندازی سرور

1.  دستور `phantom-tunnel` را روی VPS خود اجرا کنید.
2.  گزینه `1` (Server Mode) را انتخاب کنید.
3.  به سوالات ساده‌ای که پرسیده می‌شود پاسخ دهید. می‌توانید از مقادیر پیش‌فرض استفاده کنید:

    ```text
    --- 👻 Server Setup ---
    Enter Tunnel Port (for client to connect):
    Enter Public Port (for users to access):
    Enter Secret URL Path [/a1b2c3d4]:

    Checking for SSL certificate...
    SSL certificate not found. Generating a new one...
    ✅ SSL certificate 'server.crt' and 'server.key' generated successfully.
    ```
    **سرور شما آماده است!**

### ۲. راه‌اندازی کلاینت

1.  دستور `phantom-tunnel` را روی ماشین دوم (کلاینت) اجرا کنید.
2.  گزینه `2` (Client Mode) را انتخاب کنید.
3.  اطلاعات سرور و سرویس محلی خود را وارد کنید:

    ```text
    --- 👻 Client Setup ---
    Enter Server IP or Hostname []: 1.2.3.4
    Enter Server Tunnel Port:
    Enter Server Secret Path [/a1b2c3d4]:
    Enter Local Service Address (e.g. localhost:3000) [localhost:3000]:
    ```
    **کلاینت شما متصل شد!**

اکنون تونل شما به صورت کاملاً خودکار و امن در حال کار است.


## 📢 ارتباط با ما و حمایت مالی
 
برای دریافت بروزرسانی‌ها، آموزش‌ها و پاسخ به سوالات، به کانال تلگرام ما بپیوندید:

👉 [کانال تلگرام وب ویزارد](https://t.me/WebWizardsTeam)
 
اگر از این پروژه لذت بردید و مایلید از توسعه آن حمایت کنید، می‌توانید به آدرس زیر کمک مالی ارسال کنید:
 
💸 **حمایت مالی ( TRX - درگاه پرداخت ):** `TJCanxYR3GtpMkpAzxTAmmd6Szoc2asoq7`

<a href="https://www.coffeebede.com/nitroserver"><img class="img-fluid" src="https://coffeebede.ir/DashboardTemplateV2/app-assets/images/banner/default-yellow.svg" /></a>
