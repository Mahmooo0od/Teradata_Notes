# 📦 Data_Stream_Architecture (DSA)

## يعني إيه DSA بالبلدي؟

الـ **DSA** هي المكون المسئول عن إدارة عمليات النسخ الاحتياطي واسترجاع البيانات للـDatabases في Teradata ... و العمليات دي ليها اسم بيتقال و هو عمليات الـ **Backup_and_Restore (BAR)** .

---

## 🏗️ أنواع وطرق التشغيل (Deployment Types)

بيتم تقسيم التشغيل لنوعين أساسيين على حسب مكان التخزين:

1. **لـ DSU (Data_Stream_Utility):**
   وده لما بنكون بنعمل الـ Backup بتاعنا على الـ **Cloud** (زي AWS, Azure, أو GCP).

2. **لـ DSE (Data_Stream_Engine):**
   وده في الـ **On-Premises / Local** لما بنستخدم أجهزة وتطبيقات تخزين خارجية كـ NetBackup أو كـ Dell_Data_Domain أو الـ Tape_Drives.

---

## 🧩 المكونات الرئيسية للـ DSA (Core Components)

أي نظام DSA بغض النظر عن نوعه بيتكون من 3 مكونات رئيسية:

1. **الـ DSC (Data_Stream_Controller):**
   ده يعتبر **"العقل المدبر"** للسيستم فـ هو اللي بيستقبل أوامر الـ Backup و بيعمل Schedule للتسكات و بيدير الـDatabase

2. **الـ Media_Server / Client_Handler:**
   ده يعتبر **"المنفذ الفعلي"** فـ هو المسؤول إنه يسحب البيانات من قواعد Teradata ويكتبها بالفعل على أجهزة التخزين سواء كانت Local أو على الـ Cloud

3. **الـ BARCmdline & Viewpoint:**
   دي **"الواجهات"** اللي بتتعامل معاها .. سواء كنت بتفضل تشغيل الأوامر عن طريق الـ CLI بواسطة أمر كـ BARCmdline، أو من خلال الشاشات الرسومات كـ GUI عن طريق واجهة Teradata_Viewpoint

---

⬅️ [الرجوع للدرس السابق: SMWeb](01-smweb.md) | ➡️ [الرجوع للفهرس الرئيسي](../README.md) | ➡️ [الموضوع التالي: Viewpoint](../03-viewpoint.md)

