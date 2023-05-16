<p align="center">
<picture>
</picture>
  </p> 
<h1 align="center"/>X Panel</h1>
<h6 align="center">X Panel SSH User Management<h6>
<p align="center">
</p>


### فهرست
- [معرفی](#معرفی)<br>
- [امکانات](#امکانات)<br>
- [نصب](#نصب) <br>
- [بهینه سازی سرور](#بهینه-سازی-سرور)<br>
- [فعال سازی SSL](#فعال-سازی-ssl)<br>
 
## معرفی <br>
ایکس پنل یک نرم افزار تحت وب جهت مدیریت اکانت SSH می باشد. با کمک پنل تحت وب ایکس پنل می توانید کاربران را مدیریت کرده و محدودیت اعمال کنید.


## امکانات <br>
:green_circle: ایجاد کاربر بدون محدودیت <br>
:green_circle: اعمال محدودیت در حجم مصرفی و تاریخ انقضا<br>
:green_circle: قابلیت محاسبه تاریخ انقضا در اولین اتصال<br>
:green_circle: اعمال محدودیت در چند کاربره بودن اکانت<br>
:green_circle: مشاهده کاربران آنلاین<br>
:green_circle: امکان بکاپ گیری از کاربران و ریستور بکاپ<br>
:green_circle: ربات تلگرام <br>
:green_circle: تنظیم پورت ورود برای پنل<br>
:green_circle: فیک آدرس (جلوگیری از فیلترینگ) <br>
:green_circle: محدودیت IP(جلوگیری از ورود کاربران به برخی سایت ها)<br>
:orange_circle: مولتی سرور (به زودی)<br>
:orange_circle: اتصال API (به زودی)<br>

# نصب


**سیستم عامل مورد نیاز**

Ubuntu 18+ (پیشنهادی :Ubuntu 20)<br>

اگرنسخه فعلی XPanel  شما نسخه 2 به پائین است ابتدا با دستور زیر پنل را حذف کنید.
```
rm -rf /var/www/html/
mkdir /var/www/html/
chmod 777 /var/www/html/
```
برای نصب کافیست دستور زیر را وارد کنید<br>
```
bash <(curl -Ls https://raw.githubusercontent.com/Vahid-Spacer/X-Panel-SSH-User-Management/main/install.sh --ipv4)
```

حل مشکل عدم ارتباط  تماس صوتی و تصویری در اپلیکشن
```
bash <(curl -Ls https://raw.githubusercontent.com/Vahid-Spacer/X-Panel-SSH-User-Management/master/fix-call.sh --ipv4)
```
دستور بالا را در ترمینال وارد کنید سپس برای UDPGW پورت جدید تعریف کنید بهتر است به جای پورت 7300 پورت 7301 یا 7302 را تنظیم کنید
<br>
<br>

## بهینه سازی سرور
نصب و حذف تنظیمات با دستور زیر 
```
bash <(curl -Ls https://raw.githubusercontent.com/Vahid-Spacer/X-Panel-SSH-User-Management/main/TCP-Tweaker --ipv4)
```
## فعال سازی SSL
```
bash <(curl -Ls https://raw.githubusercontent.com/Vahid-Spacer/X-Panel-SSH-User-Management/main/ssl.sh --ipv4)
```
با استفاده از دستور بالا می توانید SSL را روی پنل نصب نمائید. به نکات زیر توجه کنید <br>
1- حتما قبل از نصب SSL پنل را بروز کنید<br>
2- از هیچ دستور دیگری برای فعال سازی SSL استفاده نکنید<br>
3- دامنه یا ساب دامنه را به IP سرور متصل کنید <br>
4- دستور بالا را در ترمینال وارد کنید و مراحل نصب را پیش بروید<br>
SSL بر روی پورتی که روی پنل تعریف کرده اید نصب فعال شد. <br>
  
  ## با تشکر از :
https://github.com/Alirezad07
