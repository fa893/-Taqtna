<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>واجهة المواطن - الطاقة</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: url('https://assets.onecompiler.app/42r523uca/42y46qzpj/624e50d2bca9c6314160403c2f83bc0c.jpg') no-repeat center center fixed;
            background-size: cover;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            direction: rtl;
        }

        .container {
            width: 90%;
            max-width: 400px;
            background-color: rgba(255, 255, 255, 0.6);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        h1 {
            color: #004085;
            font-size: 24px;
            margin-bottom: 20px;
        }

        .logo {
            width: 100px;
            height: auto;
            margin-bottom: 20px;
        }

        .language-select {
            margin-bottom: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .language-label {
            margin-bottom: 10px;
            font-weight: bold;
            color: #333;
        }

        .language-dropdown {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            transition: border-color 0.3s ease;
            width: 100%;
            max-width: 200px;
        }

        .language-dropdown:focus {
            border-color: #007bff;
            outline: none;
        }

        .links {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .links a {
            display: block;
            background-color: #004085;
            color: white;
            padding: 12px;
            text-align: center;
            text-decoration: none;
            font-size: 16px;
            border-radius: 8px;
            transition: background-color 0.3s ease;
        }

        .links a:hover {
            background-color: #003366;
        }

        .footer {
            margin-top: 20px;
            font-size: 14px;
            color: #6c757d;
        }

        .footer a {
            color: #004085;
            text-decoration: none;
        }

        .footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://assets.onecompiler.app/42r523uca/42y483j3a/JO%20(2).png" alt="شعار" class="logo">
        <h1 id="title">واجهة المواطن - الطاقة</h1>
        <div class="language-select">
            <label class="language-label" for="language">اختر اللغة / Select Language:</label>
            <select id="language" class="language-dropdown" onchange="changeLanguage()">
                <option value="ar">العربية</option>
                <option value="en">English</option>
            </select>
        </div>
        <div class="links">
            <a href="https://fa893.github.io/2/" target="_blank" class="link-request">نموذج طلب دعم</a>
            <a href="https://fa893.github.io/3/" target="_blank" class="link-suggestion">نموذج تقديم اقتراح</a>
            <a href="https://fa893.github.io/6/" target="_blank" class="link-payment">دفع خدمات الكهرباء والطاقة</a>
            <a href="https://fa893.github.io/1/" target="_blank" class="link-companies">شركات الطاقة الشمسية في الأردن</a>
            <a href="https://fa893.github.io/4/" target="_blank" class="link-projects">قائمة مشاريع الطاقة في الأردن</a>
            <a href="https://fa893.github.io/5/" target="_blank" class="link-authorities">الجهات الحكومية المعنية بالطاقة والكهرباء</a>
        </div>
        <div class="footer">
            <p id="footer-text">© 2024 جميع الحقوق محفوظة.</p>
        </div>
    </div>

    <script>
        function changeLanguage() {
            const language = document.getElementById('language').value;
            const title = document.getElementById('title');
            const footerText = document.getElementById('footer-text');

            if (language === 'en') {
                title.textContent = 'Citizen Interface - Energy';
                document.querySelector('.link-request').textContent = 'Support Request Form';
                document.querySelector('.link-suggestion').textContent = 'Suggestion Submission Form';
                document.querySelector('.link-payment').textContent = 'Electricity and Energy Payment Services';
                document.querySelector('.link-companies').textContent = 'Solar Energy Companies in Jordan';
                document.querySelector('.link-projects').textContent = 'List of Energy Projects in Jordan';
                document.querySelector('.link-authorities').textContent = 'Government Entities Concerned with Energy and Electricity';
                footerText.textContent = '© 2024 All rights reserved.';
                document.body.dir = "ltr";
            } else {
                title.textContent = 'واجهة المواطن - الطاقة';
                document.querySelector('.link-request').textContent = 'نموذج طلب دعم';
                document.querySelector('.link-suggestion').textContent = 'نموذج تقديم اقتراح';
                document.querySelector('.link-payment').textContent = 'دفع خدمات الكهرباء والطاقة';
                document.querySelector('.link-companies').textContent = 'شركات الطاقة الشمسية في الأردن';
                document.querySelector('.link-projects').textContent = 'قائمة مشاريع الطاقة في الأردن';
                document.querySelector('.link-authorities').textContent = 'الجهات الحكومية المعنية بالطاقة والكهرباء';
                footerText.textContent = '© 2024 جميع الحقوق محفوظة.';
                document.body.dir = "rtl";
            }
        }
    </script>
</body>
</html>
