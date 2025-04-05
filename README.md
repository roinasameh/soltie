<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>soltie</title>
  <!-- إضافة الفافايكون -->
  <link rel="icon" href="jen.jpg" type="image/jpeg">
  <style>
    body {
      background-color: #f5e9d5;
      font-family: 'Arial', sans-serif;
      padding: 30px;
      display: flex;
      justify-content: center;
      position: relative;
      overflow: auto;
      min-height: 100vh;
    }

    .container {
      max-width: 700px;
      background: rgba(255, 255, 255, 0.95);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
      z-index: 1;
    }

    img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 20px;
    }

    .emoji {
      text-align: center;
      font-size: 35px;
      margin-bottom: 20px;
    }

    p {
      font-size: 17px;
      color: #333;
      line-height: 2;
      white-space: pre-wrap;
    }

    /* استعلام وسائط للتصميم المتجاوب */
    @media (max-width: 768px) {
      body {
        padding: 15px;
      }

      .container {
        width: 90%;
        padding: 20px;
      }

      img {
        width: 100%;
      }

      .emoji {
        font-size: 25px;
      }

      .icon-button, .spotify-icon {
        width: 40px;
        height: 40px;
      }
    }

    /* استايل جديد للصورة التي ستظهر عند الضغط */
    .icon-button {
      width: 50px;
      height: 50px;
      background-image: url('pixel.jpg');
      background-size: cover;
      background-position: center;
      border-radius: 50%;
      cursor: pointer;
      margin-right: 20px;
    }

    .spotify-icon {
      width: 50px;
      height: 50px;
      cursor: pointer;
    }

    /* ترتيب الأيقونات جنب بعض */
    .icons-container {
      display: flex;
      align-items: center;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="emoji">🤍</div>
    <img src="jenlisa.jpg" alt="صورة">
    <p>
      أنا آسفة عشان ضايقتك بالكلام، وأسلوبي كان وحش.. مكنش قصدي والله.
      كنت متغاظة من فكرة إني ممكن أكون هبلة واتضحك عليّا زي ما حصلي قبل كده.

      أنا آسفة، متزعليش مني بجد.
      وعارفة إن مهما اعتذرت، مش هيصلّح اللي حصل، ومليش حق أزعل من كلامك اللي قولتيه ليا النهارده، لأنّي أنا كمان كنت كده امبارح.

      بس مش هقدر أنكر إني متضايقة، وفي كلام ضايقني فعلاً.. خصوصًا إني زي العادة، طلعت واهمة نفسي بحاجات مش حقيقية.
      متوقعتش.. ولا 1%، خصوصًا وإنك قولتيلي إني بعمل اللي عليا وزيادة.

      يا ريتك قولتي الحقيقة بدل ما تتعاملي معايا كده.

      أنا شرحت وجهة نظري.. وانتي حرة. حابة تتكلمي ونصلح؟ ولا تكتفي باللي حصل؟ 
      أنا كده كده هطنش وأنسى، لأني زي ما قلت، ماليش حق أزعل.

      بس متزعليش مني.. أنا والله بحبك، حتى لو دلوقتي كلامي باين كأنه كدب بعد اللي شُفتيه مني.
      بس ده حقك، ومش هلومك.

      أتمنى إنك تسامحيني، ولو حتى بعد ما تعاتبيني وتطلعي كل اللي جواكي.
      أنا عندي استعداد أسمعك كل يوم واعتذرلك كل يوم.. بس تسامحيني.

      أنا آسفة بجد.. وياريت متشليش مني حاجة أبداً.
    </p>

    <!-- الأيقونات جنب بعض -->
    <div class="icons-container">
      <!-- أيقونة سبوتيفاي -->
      <a href="https://open.spotify.com/playlist/3Tu7z27cJaeJqnkDsRoe69?si=be37af1438ef4307" target="_blank">
        <img src="spotify.jpg" alt="Spotify" class="spotify-icon">
      </a>

      <!-- صورة القلب -->
      <div class="icon-button" onclick="toggleText()"></div>
    </div>

    <!-- عند الضغط على الصورة يظهر النص -->
    <p id="soltie-text" style="display: none; font-size: 24px; color: pink; font-family: 'Arial', sans-serif; text-align: center; margin-top: 20px;">
      soltie
    </p>

    <script>
      function toggleText() {
        const soltieText = document.getElementById('soltie-text');
        if (soltieText.style.display === 'none') {
          soltieText.style.display = 'block';
        } else {
          soltieText.style.display = 'none';
        }
      }
    </script>
  </div>
</body>
</html>
