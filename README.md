# khidma-dz <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>خدمة DZ</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffffff;
      color: #222;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #e53935;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .section {
      padding: 20px;
      border-bottom: 1px solid #eee;
    }
    .title {
      color: #388e3c;
      font-size: 20px;
      margin-bottom: 10px;
    }
    .button {
      display: inline-block;
      padding: 10px 15px;
      background-color: #388e3c;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      margin-top: 10px;
    }
    .footer {
      text-align: center;
      padding: 15px;
      font-size: 14px;
      color: #666;
      background: #f1f1f1;
    }
  </style>
</head>
<body>

  <header>
    <h1>خدمة DZ</h1>
    <p>منصة لربط أصحاب الحرف بالزبائن</p>
  </header>

  <div class="section">
    <div class="title">🔍 البحث عن حرفي</div>
    <p>اكتشف الحرفيين في منطقتك حسب نوع الخدمة (كهربائي، نجار، ميكانيكي...)</p>
    <a href="#" class="button">ابدأ البحث</a>
  </div>

  <div class="section">
    <div class="title">🛠️ تسجيل الحرفيين</div>
    <p>هل أنت حرفي؟ أنشئ حسابك وابدأ في تلقي الطلبات!</p>
    <a href="#" class="button">سجل الآن</a>
  </div>

  <div class="section">
    <div class="title">⭐ التقييمات والآراء</div>
    <p>اطلع على تقييمات الزبائن وتحقق من جودة الخدمة.</p>
  </div>

  <div class="footer">
    &copy; 2025 خدمة DZ - كل الحقوق محفوظة
  </div>

</body>
</html>
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تسجيل الحرفيين</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>تسجيل الحرفيين</h1>
        <p>مرحبًا بك في صفحة تسجيل الحرفيين. إذا كنت حرفيًا ترغب في الانضمام إلى مجتمعنا، يرجى ملء النموذج التالي.</p>

        <form action="/submit" method="POST" enctype="multipart/form-data">
            <label for="name">الاسم الكامل:</label>
            <input type="text" id="name" name="name" required>

            <label for="phone">رقم الهاتف:</label>
            <input type="tel" id="phone" name="phone" required>

            <label for="email">البريد الإلكتروني:</label>
            <input type="email" id="email" name="email" required>

            <label for="specialty">الاختصاص أو الحرفة:</label>
            <select id="specialty" name="specialty" required>
                <option value="نجار">نجار</option>
                <option value="كهربائي">كهربائي</option>
                <option value="سباك">سباك</option>
                <!-- أضف المزيد من الحرف هنا -->
            </select>

            <label for="experience">مدة الخبرة:</label>
            <select id="experience" name="experience" required>
                <option value="1-3">1-3 سنوات</option>
                <option value="4-6">4-6 سنوات</option>
                <option value="7+">7 سنوات وأكثر</option>
            </select>

            <label for="location">الموقع (المدينة/المنطقة):</label>
            <input type="text" id="location" name="location" required>

            <label for="id_card">صورة من بطاقة الهوية:</label>
            <input type="file" id="id_card" name="id_card" accept="image/*" required>

            <label for="certificates">صورة من الشهادات أو تراخيص العمل:</label>
            <input type="file" id="certificates" name="certificates" accept="image/*" required>

            <label for="notes">ملاحظات إضافية:</label>
            <textarea id="notes" name="notes"></textarea>

            <p>قبل التسجيل، يرجى قراءة <a href="/terms">شروط الاستخدام</a>.</p>

            <button type="submit">تسجيل الآن</button>
        </form>
    </div>
</body>
</html>
/* ملف styles.css */
body {
    font-family: Arial, sans-serif;
    direction: rtl;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

.container {
    max-width: 800px;
    margin: 50px auto;
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1 {
    text-align: center;
    color: #333;
}

form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

label {
    font-size: 16px;
    color: #333;
}

input, select, textarea {
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 4px;
    width: 100%;
    box-sizing: border-box;
}

textarea {
    resize: vertical;
    height: 100px;
}

button {
    padding: 10px;
    background-color: #4CAF50;
    color: white;
    font-size: 18px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}

p {
    text-align: center;
    font-size: 14px;
    color: #777;
}
