---
title: LINUX "Cover Your Tracks" Commands
date: 2023-2-8 10:00:00 -500
categories: [Linux Commands]
tags: [Red team]     # TAG names should always be lowercase
---

<div markdown="1" style="text-align:center; font-size: 15pt;">
السلام عليكم ورحمة الله وبركاتة
<br><br>

# Cover Your Tracks

</div>

<div align="right" markdown="1" style="font-size: 15pt; color: white;">

بعد كل عملية اختبار اختراق او (Red Teaming) ممكن تحتاج تخفي اثرك وهنا بكتب بعض الاوامر الي ممكن إنها تساعدك. (^_^)
<br><br>

```Bash
echo "" > /var/log/auth.log
```
يعمل مسح لي محتوى ملف `auth.log`.
<br><br>

```Bash
echo "" > ~/.bash_history
```
يعمل مسح لي محتوى ملف `.bash_history` الخاص بالمتسخدم الحالي.
<br><br>

```Bash

rm ~/.bash_history -rf

```
بحذف الملف `.bash_history` كليًا
<br><br>

```Bash
history -c 
```
تنظيف `session history`
<br><br>

```Bash
export HISTFILESIZE=0
```
تخلي اقصى عدد صفوف 0 لي `history`
<br><br>

```Bash
export HISTSIZE=0
```
اقصى عدد للأومر الي يتم تسجيلها في `histroy` يساوي 0.
<br><br>

```Bash
unset HISTFILE
```
يعطل تسجيل الـ `history` **يحتاج انك تسجل خروج**
<br><br>

 ```Bash
 kill -9 $$
 ```
 يطفي الجلسة الحالية
 <br><br>

 ```Bash
 ln /dev/null ~/.bash_history -sf
 ```
 دايمًا يرسل اوامر `bash history` للـ `/dev/null`
 <br><br>

 <div style="text-align:center">
ان شاء الله انك استفدت معلومة ولو بسيطة<br>
شاكر لك مرورك🖤
<div>

</div>
