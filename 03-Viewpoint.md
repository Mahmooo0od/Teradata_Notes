# 📊 Teradata_Viewpoint

## يعني إيه Teradata_Viewpoint بالبلدي؟

الـ **Teradata_Viewpoint** شبه جداً Grafana كأداة عرض 
---

## ❓ ليه Teradata_Viewpoint أكتر من مجرد شاشة مراقبة كـ Grafana؟

لو بتسأل نفسك: *"ما نحط Dashboards على كـ Grafana وخلاص!"*.. الفرق الجوهري بيتلخص في 3 نقاط:

1. **التحكم والـ Administration (مش بس Monitoring):**
   * كـ Grafana في الأصل أداة عرض ومراقبة كـ **Visualization_Tool**.
   * أما كـ Viewpoint فهو **Monitoring + Administration**؛ يعني مش بس بتشوف المشكلة، انت تقدر تاخد **Action** مباشر على الداتابيز، زي إنك تعمل **Abort** لـ Query معطلة السيرفر، أو تعدل الـ Priority بتاعة Job معينة عبر قواعد كـ TASM أو كـ TIWM.

2. **عمق البيانات الخاصة بـ Teradata:**
   * الـ Viewpoint فاهم التفاصيل الداخلية المعقدة لـ Teradata جداً؛ زي توزيع العمل على الـ AMPs، ومشاكل الـ **Data_Skew**، الـ **Spool_Space** المجهد، مين عامل **Lock** على جدول مين، وحتى تفاصيل الـ **Explain_Plan** لكل استعلام شغال.

3. **خاصية العودة بالزمن (Rewind Feature):**
   * دي ميزة جبارة؛ لو حصلت مشكلة الساعة 3 الفجر والسيستم وقع أو تباطأ، تقدر الصبح ترجع بالزمن لشاشة المراقبة زي ما كانت بالظبط الساعة 3 الفجر وتشوف مين الـ Query أو الـ User اللي تسبب في المشكلة.

---

## 🧩 فكرة عمل الشاشة (Portlets and Portals)

شاشة الـ Viewpoint بتتكون من أجزاء بسيطة بتسهل تخصيصها:

* **كـ Portlets:** دي عبارة عن الـ Widgets أو التطبيقات الصغيرة المستقلة (زي Portlet لمراقبة الـ System_Health، وPortlet لتتبع الـ Locks، وPortlet للـ Active_Queries).
* **كـ Roles / Customization:** كل مستخدم (سواء DBA، Data_Engineer، أو Management) يقدر يظبط الـ Dashboard بتاعته ويحط الـ Portlets اللي تهتم بشغله فقط.

---

## 💡 باختصار:
كـ Grafana هو أداة مراقبة عامة وممتازة لأي سيستم، أما كـ Viewpoint فهو شاشة المراقبة + غطاء التحكم الكامل كـ **Control_Center** الخاص بنظام Teradata.

---

⬅️ [الرجوع للدرس السابق: DSA](02-dsa.md) | ➡️ [الرجوع للفهرس الرئيسي](../README.md) | ➡️ [الموضوع التالي: System Architecture](04-system-architecture/01-amp-and-bynet.md)

