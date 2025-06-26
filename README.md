# landing-page
landing-page
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>انطلق مع منتجك الرقمي</title>
  <style>
    body {
      margin: 0;
      font-family: 'Tahoma', sans-serif;
      direction: rtl;
      background: #f9f9f9;
    }
    .container {
      max-width: 700px;
      margin: auto;
      padding: 40px 20px;
      background: #fff;
      text-align: center;
      box-shadow: 0 5px 25px rgba(0,0,0,0.1);
      margin-top: 60px;
      border-radius: 12px;
    }
    h1 {
      color: #1d3557;
      font-size: 32px;
    }
    p {
      color: #444;
      font-size: 18px;
      margin: 20px 0;
    }
    .cta-button {
      background: #457b9d;
      color: white;
      padding: 14px 28px;
      text-decoration: none;
      border: none;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
      margin-top: 20px;
      transition: background 0.3s ease;
    }
    .cta-button:hover {
      background: #1d3557;
    }
    form {
      margin-top: 30px;
    }
    input[type="email"] {
      padding: 12px;
      width: 80%;
      max-width: 400px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 16px;
    }
    input[type="submit"] {
      margin-top: 15px;
      background-color: #e63946;
      color: white;
      border: none;
      padding: 12px 25px;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }
    input[type="submit"]:hover {
      background-color: #d62828;
    }
    @media (max-width: 600px) {
      h1 {
        font-size: 24px;
      }
      p {
        font-size: 16px;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>أطلق مشروعك الرقمي الآن 🚀</h1>
    <p>سجل بريدك الإلكتروني لتكون أول من يحصل على تحديثاتنا وتجربة مجانية للمنتج.</p>
    
    <a href="#form" class="cta-button">ابدأ مجانًا</a>

    <form id="form" onsubmit="return submitForm(event)">
      <input type="email" id="email" placeholder="أدخل بريدك الإلكتروني" required />
      <br>
      <input type="submit" value="سجّل الآن" />
    </form>

    <p id="success" style="color: green; display: none; margin-top: 20px;">✅ تم التسجيل بنجاح!</p>
  </div>

  <script>
    function submitForm(event) {
      event.preventDefault();
      const email = document.getElementById("email").value;
      if (email) {
        // فقط للتجربة المحلية، بدون إرسال فعلي
        document.getElementById("success").style.display = "block";
        document.getElementById("form").reset();
      }
    }
  </script>

</body>
</html>
