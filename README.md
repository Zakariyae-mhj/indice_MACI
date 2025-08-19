مؤشر MACI (Moisture Adjusted Chlorophyll Index)
🔎 تعريف

مؤشر MACI هو مؤشر طيفي يُستخدم لتقدير حالة الغطاء النباتي من خلال دمج معلومات الكلوروفيل مع تأثير الرطوبة في الغطاء الأرضي. يتيح هذا المؤشر مراقبة الإجهاد النباتي بشكل أكثر دقة مقارنة بالمؤشرات التقليدية، خاصة في البيئات الجافة وشبه الجافة.

🧮 المعادلة

يعتمد مؤشر MACI على الصيغة التالية:

𝑀
𝐴
𝐶
𝐼
=
(
𝑁
𝐼
𝑅
−
𝑅
𝑒
𝑑
)
/
(
𝑁
𝐼
𝑅
+
𝑅
𝑒
𝑑
+
𝑆
𝑊
𝐼
𝑅
)
MACI=(NIR−Red)/(NIR+Red+SWIR)

حيث:

NIR : النطاق القريب من تحت الأحمر (Near Infrared)

Red : النطاق الأحمر (Red band)

SWIR : النطاق تحت الأحمر قصير الموجة (Shortwave Infrared)

⚙️ المنهجية

تحميل صور الأقمار الصناعية (مثل Sentinel-2).

إجراء عمليات المعالجة المسبقة (تصحيح الغلاف الجوي، القص على مجال الدراسة).

استخراج القنوات الطيفية (Red, NIR, SWIR).

تطبيق معادلة MACI بداخل Google Earth Engine أو Python.

توليد الخرائط والنتائج على شكل خرائط مؤشر.

📂 متطلبات التشغيل

حساب على Google Earth Engine

أو بيئة Python مع المكتبات:

geemap

numpy

rasterio

matplotlib

▶️ كيفية الاستخدام

نسخة Google Earth Engine:

افتح كود المؤشر من هذا المستودع.

الصق الكود داخل محرر GEE.

حدد مجال الدراسة والفترة الزمنية.

نفّذ البرنامج لعرض خرائط MACI.

نسخة Python:

نزّل الصور (Sentinel-2 L2A).

افتح ملف الـ .py المرفق.

حدّث المسار إلى مكان تخزين الصور.

نفّذ الكود للحصول على النتائج.

📝 المخرجات

خرائط مؤشر MACI بصيغة GeoTIFF.

رسوم بيانية لتغير المؤشر عبر الزمن.

إمكانية دمج النتائج مع مؤشرات أخرى مثل NDVI وMSI.

📚 المراجع

Haboudane, D., et al. (2004). Hyperspectral vegetation indices and novel algorithms for predicting green LAI of crop canopies. Remote Sensing of Environment.

Gao, B. (1996). NDWI—A normalized difference water index for remote sensing of vegetation liquid water. Remote Sensing of Environment.
