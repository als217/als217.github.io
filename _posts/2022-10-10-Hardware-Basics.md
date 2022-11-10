---
title: Hardware Basics
date: 2022-10-10 10:00:00 -500
categories: [Hardware Basics, Hardware Security]
tags: [Hardware, Hardware Basics, Red team]     # TAG names should always be lowercase
---
<style>
    body{
        background-color: #0f0e15
    }
    .cont {
        position: relative;
        text-align: center;
        color: white;
    }
    .centered {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .insetshadow {
        color: #fff;
        letter-spacing: .2em;
        text-shadow: 
        -4px -4px 4px #111, 
        6px 6px 6px #363636;
        font-weight:750;
        font-size:50pt;
    }
    .rotate90 {
        -webkit-transform: rotate(270deg);
        -moz-transform: rotate(270deg);
        -o-transform: rotate(270deg);
        -ms-transform: rotate(270deg);
        transform: rotate(270deg);
    }
    .title{
    color:#4BB59B;
    font-weight: bold;
    background-color:;
    padding:5px;
    }   
</style>
<div class="cont">
    <img class="rotate90" src="https://github.com/als217/als217.github.io/blob/main/Images/Hardware_Basics.jpg?raw=true" alt="Background image" style="width:75%;opacity: 0.4;">
    <p class="centered insetshadow" fill="#fff">Hardware Basics</p>
</div>
<div markdown="1" style="font-size: 15pt" align="center">
            
------------------------------------
# **السلام عليكم ورحمة الله وبركاتة**

مساء او صباح الخير على حسب توقيتك عزيزي,  طبعا المقالة هاذي بالعربي والكلام ممكن يكون بصيغة عامية فا نأخذ على
.😆بعضنا شويا

</div>

<blockquote>
<h2 class="title">Content</h2>
<blockquote >
<div markdown="1" style="font-size: 15pt; color: white;">

* What is PCB and Embedded devices?
* What is the difference between a Micorcontroller and Micorprocessor?
* What are the common Types of CPU Architecture?
* What are the common Types of Storge?
* What are Types of System Structure?
* What are the common Types of Protocols Bus?

</div>
</blockquote>
</blockquote>

<img src="https://github.com/als217/als217.github.io/blob/main/Images/Mems.jpg?raw=true" alt="Just Memes">
--------------------------


<blockquote>
<h2 class="title">PCB and Embedded Devices</h2>
</blockquote>
<div align="right" style="font-size: 14pt;">
<p>
<strong>Printect Circuit Board</strong> اختصار لي <strong>PCB</strong><br>
تشير الى البورد الخضراء التي يتم من خلالها توصيل جميع القطع الالكترونية والكهربائية ببعضها البعض عن طريق اللحام والحفر وغيرها. </p> 
<p>
<strong> Embedded Devices</strong><br>
او الانظمة المظمنة وهيا انظمة دمجت المعالج والذاكرة والادخال والاخراج وغيرها مع بعضها البعض, ونظام التشغيل مدمج معاها,  صممت لتنفيذ وظيفة محدده او اكثر من وظيفة, على سبيل المثال الراوتير, الساعات الذكية, والشاشات الذكية وغيرها. </p>
</div>

--------------------------

<blockquote>
<h2 class="title">Micorcontroller VS Micorprocessor</h2>
</blockquote>
<div align="right" style="font-size: 14pt;">
<p><strong>Micorocontroller</strong><br>
كمبيوتر صغير مدمج في شريحة وحده موجود فيها كل الوظايف الي يحتاجها مثل الذاكرة العشوائية والمداخل والمخارج, يتسخدم في الاردوينو وبعض المشاريع, ويتعامل مع بيانات صغيرة الحجم <br>
<strong> (IC Integrated Circuit) </strong>ويكون داخل ال 
<br>
<strong>Atmel AVR</strong>  مثل 
<br>
</p>
<p><strong>Microprocessor</strong><br>
وهذا الي نعرفه ونستخدمه في اجهزتها الي هوا المعالج او وحدة المعالجة المركزية, والاختلاف هنا ان الوظايف الي ذكرنها سابقا تكون موصله له وليست مدمجه داخلة.
<br>
<strong>intel I7</strong>  مثل 
<br>
</p>
صورة توضح الفرق بينهم:

<img src="https://github.com/als217/als217.github.io/blob/main/Images/Microvsprocr.jpg?raw=true" alt="Microcontroller vs MicroProcessor"><br><br>

<p><strong>SOC - System On Chip</strong><br>
وهاذي نقدر انها شبيها بي الاثنين الي اخذناهم, بحيث ان فيها جميع الدوائر الالكترونية الازمة وفيها نظام تشغيل بداخلها عكسهم وايضا يتعامل مع بيانات كبيرة في الحجم. موجود على الاجهزة الي تشتغل على نظام لنيكس مثل بعض الراوترات.
<br>
<strong>Qualcomm Snapdragon</strong>  مثل 
</p>
</div>

-------------------------------


<blockquote>
<h2 class="title">CPU Architecture Types</h2>
</blockquote>
<div align="right" style="font-size: 15pt" ><p>
اشهر انواع معمارية وحدات التحكم المستخدمة </p></div>
<div style="font-size: 15pt;">
<ul>
<li>Microcontroller</li>
<ul><li>غالبا اي وحدة تحكم من شركة Atmel -> AVR</li></ul>
<li>Micorprocessor</li>
<ul>
<li>x86</li>
<li>x64</li>
</ul>
<li>SoC</li>
<ul>
<li>ARM</li>
<li>MIPS</li>
</ul>
</ul>
</div>

----------------------

<blockquote>
<h2 class="title">Storage Types</h2>
</blockquote>
<div align="right" style="font-size: 15pt"><strong>طبعا كل جهاز لازم يكون فيه مكان تتخزن فيه البيانات, وفيه انواع لي اماكن تخزين البيانات تختلف بإختلاف البيانات المراد حفظها.<br>
ثلاث انواع رئيسة حنتكلم عنها بشكل بسيط جدا<br>
</strong></div><br>
<div style="font-size: 15pt" align="right">
<ul>
<li><strong>Flash Memory</strong></li>
<ul>
<li>التخزين الي نستخدمه دايما ويدخل تحت المسمى هذا العديد من الاشياء زي الهارديسك واليو اس بي, ويستخدم لتخزين نظام معين او بيانات محدده, وفي نفس الوقت البيانات ماتروح اذا فصلت عنها الطاقه او الكهرباء. </li>
<li>NOR / NAND flash </li>
<li> وهذا يشير الى المنطق او البوابات المستخدمه داخل هذا وحدة التخزين, طبعا لكل وحده خصائصها مارح نتعمق فيها.</li>
</ul><br>
<li><strong>EEPROM</strong></li>
<ul><li>طبعا هاذي الذاكرة تكون موجودة على البورد ولايمكن انك تكتب عليها فقط للقراءة, ويتخزن فيها بيانات خاصة بالاعدادات وملفات نظام التشغيل.</li>
<li> بتسخدمها لعدة اسباب منها القراء السريعة NOR</li>
<li> بروتوكلات تستخدمها للتواصل بين القطع الاخرى (I2C, ISP)</li></ul><br>
<li><strong>RAM</strong></li>
<ul><li>ذاكرة الوصول العشوائية يتم استخدمها اثناء تشغيل الجهاز لتخزين البيانات المتعلقة بنظام التشغيل و بالبرامج من اجل تسريع معالجتها من قبل المعالج, وفي حال اغلاق الجهاز او انقطاع الطاقة يتم حذف جميع البيانات بداخلها.</li>
<li>(Static RAM - SRAM, Dynamic RAM - DRAM)في منها نوعين </li></ul></ul></div>

----

<blockquote>
<h2 class="title">System Structure</h2>
</blockquote>
<div align="right" style="font-size: 15pt">
لكل نظام او وحدة معالجة بنية تحتية للنظام يتعامل معاها حنتكلم عن اسياسيات اثنين منهم
</div>
<div style="font-size: 15pt" align="right">
<ul>
<li><strong>UBOOT</strong></li>
<ul><li>Bootloader نظام التشغيل</li>
<li>SD, USB, I2C, SPI, TFTP, NFS يدعم البروتكولات وهاذي وغيرها</li>
<li>يقراء ملفات النظام وينسخها في الذاكرة ليتم تنفيذها</li></ul>
<li><strong>ROOTFS</strong></li>
<ul><li>ملفات نظام تشغيل كالي الاعتيادية</li></ul></ul>
</div><br>

----

<blockquote>
<h2 class="title">Bus Protocols</h2>
</blockquote>
<div align="right" style="font-size: 15pt">
البروتوكولات هيا قوانين او قواعد تساعد على ان كل طرف يفهم الطرف الاخر.,<br>
طبعا لكل بروتوكل طريقة تواصل ونظام محدد وبعض المتطلبات ماراح ندخل في تفاصيلها حاليا ولاكن كويس نعرفها.
</div><br>

<div style="font-size: 15pt" align="right">
<ul>
<li><strong>I2C - Inter-integrated circuit</strong></li>
<ul><li>تقنية تسمحلك بتواصل مع اكثر من عنصر او جهاز بإستخدام اقل عدد ممكن من التوصيلات وبنفس الكفاءة, تستخدم فقط إشارتين</li></ul>
<li><strong>SPI - Serial Peripheral Interface</strong></li>
<ul><li>تسلسلي في نقل البيانات ويستخدم في المسافات القصيرة</li></ul>
<li><strong>UART - Universal Asynchronous Receiver-Transmitter</strong></li>
<ul><li>بروتوكول للارسال والاستقبال ويمكن ضبط سرعة الارسال ويستخدم في بعض الاحيان لصلاح الاخظاء </li></ul>
<li><strong>CANBUS</strong></li>
<ul><li>يستخدم غالبا في السيارات</li></ul>
<li><strong>Wiegand</strong></li>
<ul><li>RFIDيتسخدم للتحقق من اشارة البطايق او مايعرف بال</li></ul>
</ul>
</div>
-----------------


<blockquote>
<h2 class="title">References</h2>
</blockquote>
<div align="right" markdown="1" style="font-size: 15pt">
ان شاء الله اني اكون وفقت في الطرح وإنك استمتعت عزيزي القاري واستفدت <br>
المراجع الي اعتمدت عليها<br>

* Hardware Hacking HandBook
* https://en.wikipedia.org/wiki/Microcontroller 
* My special spices 😎
</div>