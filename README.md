
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Librairie PDF | متجر كتب PDF</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      background: #f4f4f4;
      margin: 0;
      padding: 40px;
    }
    .lang-switch {
      margin-bottom: 30px;
    }
    .lang-switch button {
      padding: 10px 20px;
      margin: 5px;
      cursor: pointer;
    }
    .book {
      background: #fff;
      border-radius: 10px;
      padding: 20px;
      margin: 20px auto;
      width: 300px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    .book h2 {
      margin-bottom: 10px;
    }
    .book p {
      margin: 5px 0;
    }
    .book a button {
      background-color: #4CAF50;
      color: white;
      border: none;
      padding: 10px 20px;
      margin-top: 10px;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <!-- Language Switch -->
  <div class="lang-switch">
    <button onclick="showFrench()">🇫🇷 Français</button>
    <button onclick="showArabic()">🇸🇦 العربية</button>
  </div>

  <!-- French Section -->
  <div id="french">
    <h1>Bienvenue dans notre boutique de livres PDF</h1>
    <div class="book">
      <h2>Les secrets du succès</h2>
      <p>Un guide pratique pour réussir votre vie personnelle et professionnelle.</p>
      <p>Prix: 5€</p>
      <a href="https://buy.stripe.com/test_payment_link"><button>Acheter maintenant</button></a>
    </div>
  </div>

  <!-- Arabic Section -->
  <div id="arabic" style="display:none;">
    <h1>مرحبًا بك في متجرنا لبيع كتب PDF</h1>
    <div class="book">
      <h2>أسرار النجاح</h2>
      <p>دليل عملي لتحقيق النجاح في حياتك الشخصية والمهنية.</p>
      <p>السعر: 5 يورو</p>
      <a href="https://buy.stripe.com/test_payment_link"><button>اشترِ الآن</button></a>
    </div>
  </div>

  <script>
    function showFrench() {
      document.getElementById("french").style.display = "block";
      document.getElementById("arabic").style.display = "none";
    }
    function showArabic() {
      document.getElementById("french").style.display = "none";
      document.getElementById("arabic").style.display = "block";
    }
  </script>
</body>
</html>

