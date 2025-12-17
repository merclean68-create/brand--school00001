[2مشروع تطور الدات.txt](https://github.com/user-attachments/files/24223287/2.txt)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>brand-school</title>
    <style>
        body {
            background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Mercedes-Benz_logo_2010.png/600px-Mercedes-Benz_logo_2010.png');
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center top;
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px 10px 20px 10px;
            word-break: keep-all;
            overflow-wrap: break-word;
        }

        h1, h2, h3, p {
            margin: 15px 0;
            color: #333;
        }

        button {
            margin: 10px;
            padding: 15px 25px;
            font-size: 16px;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            background-color: #0077b6;
            background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Mercedes-Benz_logo_2010.png/600px-Mercedes-Benz_logo_2010.png');
            background-size: cover;
            background-position: center;
            text-shadow: 1px 1px 2px black;
            word-break: keep-all;
            transition: transform 0.2s, box-shadow 0.2s;
        }

        button:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }

        #btn2 {
            display: none;
            margin: 10px;
            padding: 15px 25px;
            font-size: 16px;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            background-color: #0077b6;
            background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Mercedes-Benz_logo_2010.png/600px-Mercedes-Benz_logo_2010.png');
            background-size: cover;
            background-position: center;
            text-shadow: 1px 1px 2px black;
            word-break: keep-all;
            transition: all 0.5s ease;
        }

        /* صندوق الشرح */
        #infoBox {
            margin-top: 20px;
            padding: 20px;
            border-radius: 10px;
            background-color: rgba(0, 119, 182, 0.8);
            color: white;
            font-size: 16px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            display: none; /* مخفي بشكل افتراضي */
            text-align: right;
        }

        /* تصميم متجاوب */
        @media (max-width: 768px) {
            button {
                width: 90%;
                font-size: 18px;
            }

            #infoBox {
                width: 90%;
                font-size: 16px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <h1>brand-school شركة تعليم الجدب</h1>
    <h2>دورة تعليم</h2>
    <h3>قوامة الجسم</h3>

    <!-- الأزرار الرئيسية -->
    <button title="تعلم الأسلوب الفرنسي">Style France</button>
    <button title="تعلم الأسلوب العربي">Style Arabic</button>
    <button title="تعلم الأسلوب الإنجليزي">Style English</button>
    <button title="اختيار التخصص">التخصص</button>

    <!-- الزر لإظهار الزر المخفي -->
    <button onclick="showBtn()" title="اضغط لإظهار الزر المخفي">اضغط لإظهار الزر</button>
    <button id="btn2" title="اللغة + اختيار الكلمات + إرشاد إلى كتب جدب الزبون">
        اللغة + اختيار الكلمات + إرشاد إلى كتب جدب الزبون
    </button>

    <!-- أزرار الشرح -->
    <button onclick="showHindam()" title="تعلم الهندام">هندام</button>
    <button onclick="showIsharat()" title="تعلم الإشارات">الإشارات</button>
    <button onclick="showHarakat()" title="تعلم الحركات">الحركات</button>
    <button onclick="showKalam()" title="تعلم الكلام">الكلام</button>

    <!-- زر اتصل بنا -->
    <button onclick="window.location.href='mailto:your-email@example.com'" title="اتصل بنا">
        اتصل بنا
    </button>

    <!-- زر التواصل عبر فيسبوك -->
    <button onclick="window.open('https://www.facebook.com/YourPage', '_blank')" title="تواصل معنا على فيسبوك">
        فيسبوك
    </button>

    <!-- زر السعر -->
    <button onclick="showPrice()" title="السعر / الثمن">السعر</button>

    <!-- صندوق المعلومات -->
    <div id="infoBox"></div>

    <p>مرحبا بالجميع في مدرسة تعليم الجدب وتسليط الضوء</p>

    <script>
        function showBtn() {
            const btn = document.getElementById("btn2");
            btn.style.display = "inline-block";
            btn.style.opacity = 1;
        }

        const infoBox = document.getElementById("infoBox");

        function showHindam() {
            infoBox.style.display = "block";
            infoBox.innerHTML = "<strong>هندام:</strong><br>1- الجدب<br>2- طريقة لبسك للبيع أو للمقابلة أو لعملية الجدب سواء في فيديو أو واقع";
        }

        function showIsharat() {
            infoBox.style.display = "block";
            infoBox.innerHTML = "<strong>الإشارات:</strong><br>- كيفية لفت الانتباه<br>- التأثير<br>- حركات الأصابع<br>- حركات اليدين<br>- اتساق حركة اليد مع الكلام أو الصمت";
        }

        function showHarakat() {
            infoBox.style.display = "block";
            infoBox.innerHTML = "<strong>الحركات:</strong><br>- قوامة الجسم<br>- رياضة<br>- المشي<br>- كيفية الالتفات<br>- كيفية النظر<br>- كيفية الوقوف";
        }

        function showKalam() {
            infoBox.style.display = "block";
            infoBox.innerHTML = "<strong>الكلام:</strong><br>- اللغة<br>- اختيار الكلمات<br>- إرشادات إلى كتب تساعد في جدب الزبون";
        }

        function showPrice() {
            infoBox.style.display = "block";
            infoBox.innerHTML = "<strong>السعر:</strong> 300 DA";
        }
    </script>
</body>
</html>
