<html lang="fa" dir="rtl">

<head>

  <meta charset="UTF-8">

  <meta
    name="viewport"
    content="width=device-width, initial-scale=1.0">

  <title>⚡ AMIR GAMER</title>

  <meta
    name="description"
    content="AMIR GAMER | سایت گیمینگ، اخبار و خدمات">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    html{
      scroll-behavior:smooth;
    }

    body{

      font-family:
        Tahoma,
        Arial,
        sans-serif;

      background:
        radial-gradient(
          circle at 20% 10%,
          #16213d 0,
          transparent 30%
        ),
        radial-gradient(
          circle at 80% 20%,
          #321137 0,
          transparent 30%
        ),
        #050509;

      color:#fff;

      min-height:100vh;

      overflow-x:hidden;

    }


    /* =========================
       RGB BACKGROUND
    ========================= */

    body::before{

      content:"";

      position:fixed;

      inset:-50%;

      pointer-events:none;

      z-index:-1;

      background:
        conic-gradient(
          from 0deg,
          #00eaff20,
          #ff00cc18,
          #7b2cff20,
          #00ff9d15,
          #00eaff20
        );

      filter:blur(80px);

      animation:
        rgbRotate 12s linear infinite;

    }


    @keyframes rgbRotate{

      from{
        transform:rotate(0deg);
      }

      to{
        transform:rotate(360deg);
      }

    }


    /* =========================
       HEADER
    ========================= */

    header{

      position:sticky;

      top:0;

      z-index:999;

      background:
        rgba(5,5,9,.78);

      backdrop-filter:
        blur(18px);

      border-bottom:
        1px solid #ffffff12;

    }


    .navbar{

      width:92%;

      max-width:1250px;

      min-height:75px;

      margin:auto;

      display:flex;

      align-items:center;

      justify-content:space-between;

      gap:20px;

    }


    /* LOGO */

    .logo{

      display:flex;

      align-items:center;

      gap:10px;

      text-decoration:none;

      color:#fff;

      font-weight:900;

      font-size:22px;

      white-space:nowrap;

    }


    .logo-icon{

      width:43px;

      height:43px;

      display:flex;

      align-items:center;

      justify-content:center;

      border-radius:13px;

      background:
        linear-gradient(
          135deg,
          #00eaff,
          #7b2cff,
          #ff00cc
        );

      box-shadow:
        0 0 18px #00eaff55,
        0 0 35px #ff00cc22;

      animation:
        logoRGB 3s linear infinite;

    }


    @keyframes logoRGB{

      0%{
        box-shadow:
          0 0 18px #00eaff66;
      }

      50%{
        box-shadow:
          0 0 25px #ff00cc66;
      }

      100%{
        box-shadow:
          0 0 18px #00eaff66;
      }

    }


    .logo span{

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #fff,
          #ff00cc
        );

      -webkit-background-clip:text;

      background-clip:text;

      color:transparent;

    }


    /* MENU */

    nav{

      display:flex;

      align-items:center;

      gap:8px;

    }


    nav a{

      position:relative;

      padding:10px 14px;

      border-radius:10px;

      color:#aaa;

      text-decoration:none;

      font-size:14px;

      transition:.25s;

    }


    nav a:hover{

      color:#fff;

      background:#ffffff08;

    }


    nav a::after{

      content:"";

      position:absolute;

      right:14px;

      left:14px;

      bottom:4px;

      height:2px;

      border-radius:5px;

      transform:scaleX(0);

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #ff00cc
        );

      transition:.25s;

    }


    nav a:hover::after{

      transform:scaleX(1);

    }


    /* MOBILE MENU */

    .menu-btn{

      display:none;

      width:43px;

      height:43px;

      border:1px solid #ffffff18;

      border-radius:12px;

      background:#ffffff08;

      color:#fff;

      font-size:22px;

      cursor:pointer;

    }


    /* =========================
       HERO
    ========================= */

    .hero{

      width:92%;

      max-width:1250px;

      min-height:
        calc(100vh - 75px);

      margin:auto;

      display:grid;

      grid-template-columns:
        1.1fr .9fr;

      align-items:center;

      gap:50px;

      padding:
        70px 0;

    }


    .hero-content{

      animation:
        heroIn .8s ease;

    }


    @keyframes heroIn{

      from{

        opacity:0;

        transform:
          translateY(25px);

      }

      to{

        opacity:1;

        transform:
          translateY(0);

      }

    }


    .hero-badge{

      display:inline-flex;

      align-items:center;

      gap:8px;

      padding:9px 14px;

      border-radius:30px;

      border:1px solid #00eaff35;

      background:#00eaff09;

      color:#00eaff;

      font-size:12px;

      margin-bottom:20px;

    }


    .hero h1{

      font-size:
        clamp(
          42px,
          7vw,
          82px
        );

      line-height:1;

      font-weight:1000;

      letter-spacing:-3px;

    }


    .hero h1 .rgb-text{

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #7b2cff,
          #ff00cc,
          #00eaff
        );

      background-size:300% auto;

      -webkit-background-clip:text;

      background-clip:text;

      color:transparent;

      animation:
        textRGB 5s linear infinite;

    }


    @keyframes textRGB{

      to{
        background-position:
          300% center;
      }

    }


    .hero h2{

      margin-top:18px;

      color:#ddd;

      font-size:
        clamp(
          18px,
          3vw,
          28px
        );

    }


    .hero-description{

      max-width:650px;

      margin-top:20px;

      color:#888;

      line-height:2;

      font-size:15px;

    }


    /* BUTTONS */

    .hero-buttons{

      display:flex;

      flex-wrap:wrap;

      gap:12px;

      margin-top:30px;

    }


    .btn{

      display:inline-flex;

      align-items:center;

      justify-content:center;

      gap:8px;

      min-width:150px;

      padding:14px 20px;

      border-radius:13px;

      text-decoration:none;

      color:#fff;

      font-weight:bold;

      font-size:14px;

      transition:.3s;

    }


    .btn-primary{

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #7b2cff,
          #ff00cc
        );

      background-size:200%;

      box-shadow:
        0 0 25px #00eaff20;

    }


    .btn-primary:hover{

      transform:
        translateY(-3px);

      background-position:
        100%;

      box-shadow:
        0 0 35px #00eaff40;

    }


    .btn-secondary{

      border:
        1px solid #ffffff18;

      background:#ffffff07;

    }


    .btn-secondary:hover{

      border-color:#00eaff55;

      background:#00eaff08;

      transform:
        translateY(-3px);

    }


    /* =========================
       GAMING CARD
    ========================= */

    .hero-visual{

      position:relative;

      display:flex;

      justify-content:center;

      align-items:center;

    }


    .gaming-card{

      position:relative;

      width:
        min(430px,100%);

      aspect-ratio:1/1;

      border-radius:35px;

      padding:2px;

      background:
        linear-gradient(
          135deg,
          #00eaff,
          #7b2cff,
          #ff00cc,
          #00eaff
        );

      background-size:300% 300%;

      animation:
        cardRGB 6s ease infinite;

      box-shadow:
        0 0 50px #00eaff20,
        0 0 100px #ff00cc12;

    }


    @keyframes cardRGB{

      0%{
        background-position:
          0% 50%;
      }

      50%{
        background-position:
          100% 50%;
      }

      100%{
        background-position:
          0% 50%;
      }

    }


    .gaming-card-inner{

      width:100%;

      height:100%;

      display:flex;

      flex-direction:column;

      align-items:center;

      justify-content:center;

      border-radius:33px;

      background:
        radial-gradient(
          circle,
          #151a35,
          #07070d 65%
        );

      overflow:hidden;

      position:relative;

    }


    .gaming-card-inner::before{

      content:"";

      position:absolute;

      width:220px;

      height:220px;

      border-radius:50%;

      background:#00eaff;

      filter:blur(100px);

      opacity:.15;

    }


    .controller{

      font-size:
        clamp(
          90px,
          15vw,
          150px
        );

      position:relative;

      filter:
        drop-shadow(
          0 0 20px #00eaff66
        );

      animation:
        floatController 3s ease-in-out infinite;

    }


    @keyframes floatController{

      0%,100%{
        transform:
          translateY(0)
          rotate(-3deg);
      }

      50%{
        transform:
          translateY(-15px)
          rotate(3deg);
      }

    }


    .gaming-card h3{

      margin-top:15px;

      font-size:25px;

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #fff,
          #ff00cc
        );

      -webkit-background-clip:text;

      background-clip:text;

      color:transparent;

    }


    .gaming-card p{

      margin-top:8px;

      color:#777;

      font-size:13px;

    }


    /* FLOATING RGB DOTS */

    .rgb-dot{

      position:absolute;

      width:8px;

      height:8px;

      border-radius:50%;

      background:#00eaff;

      box-shadow:
        0 0 15px #00eaff;

      animation:
        dotFloat 4s ease-in-out infinite;

    }


    .dot1{

      top:10%;

      right:5%;

    }


    .dot2{

      bottom:15%;

      left:0;

      background:#ff00cc;

      box-shadow:
        0 0 15px #ff00cc;

      animation-delay:1s;

    }


    .dot3{

      top:40%;

      left:-10%;

      background:#7b2cff;

      box-shadow:
        0 0 15px #7b2cff;

      animation-delay:2s;

    }


    @keyframes dotFloat{

      0%,100%{
        transform:
          translateY(0);
      }

      50%{
        transform:
          translateY(-20px);
      }

    }


    /* =========================
       FEATURES
    ========================= */

    .features{

      width:92%;

      max-width:1250px;

      margin:auto;

      padding:
        20px 0 100px;

    }


    .section-title{

      text-align:center;

      margin-bottom:35px;

    }


    .section-title span{

      font-size:30px;

      font-weight:900;

      background:
        linear-gradient(
          90deg,
          #00eaff,
          #fff,
          #ff00cc
        );

      -webkit-background-clip:text;

      background-clip:text;

      color:transparent;

    }


    .section-title p{

      margin-top:10px;

      color:#777;

      font-size:13px;

    }


    .feature-grid{

      display:grid;

      grid-template-columns:
        repeat(
          3,
          1fr
        );

      gap:18px;

    }


    .feature-card{

      padding:28px;

      border-radius:20px;

      background:#ffffff05;

      border:
        1px solid #ffffff12;

      transition:.3s;

    }


    .feature-card:hover{

      transform:
        translateY(-7px);

      border-color:
        #00eaff44;

      background:
        #00eaff07;

      box-shadow:
        0 0 30px #00eaff0d;

    }


    .feature-icon{

      width:55px;

      height:55px;

      display:flex;

      align-items:center;

      justify-content:center;

      border-radius:15px;

      font-size:25px;

      background:
        linear-gradient(
          135deg,
          #00eaff15,
          #ff00cc15
        );

      border:
        1px solid #ffffff12;

      margin-bottom:18px;

    }


    .feature-card h3{

      font-size:18px;

      margin-bottom:10px;

    }


    .feature-card p{

      color:#777;

      line-height:1.9;

      font-size:13px;

    }


    /* =========================
       FOOTER
    ========================= */

    footer{

      margin-top:50px;

      border-top:
        1px solid #ffffff12;

      background:#030306;

    }


    .footer-inner{

      width:92%;

      max-width:1250px;

      margin:auto;

      padding:35px 0;

      display:flex;

      align-items:center;

      justify-content:space-between;

      gap:20px;

    }


    .footer-copy{

      color:#666;

      font-size:12px;

    }


    .footer-brand{

      color:#00eaff;

      font-weight:bold;

    }


    /* =========================
       MOBILE
    ========================= */

    @media(max-width:850px){

      .menu-btn{

        display:block;

      }


      nav{

        position:absolute;

        top:75px;

        right:4%;

        left:4%;

        display:none;

        flex-direction:column;

        align-items:stretch;

        padding:10px;

        border-radius:16px;

        background:
          rgba(7,7,13,.96);

        border:
          1px solid #ffffff12;

      }


      nav.active{

        display:flex;

      }


      nav a{

        text-align:center;

      }


      .hero{

        grid-template-columns:1fr;

        text-align:center;

        padding-top:50px;

      }


      .hero-description{

        margin-left:auto;

        margin-right:auto;

      }


      .hero-buttons{

        justify-content:center;

      }


      .hero-visual{

        order:-1;

      }


      .gaming-card{

        width:
          min(360px,90vw);

      }


      .feature-grid{

        grid-template-columns:1fr;

      }


      .footer-inner{

        flex-direction:column;

        text-align:center;

      }

    }


    @media(max-width:450px){

      .navbar{

        width:94%;

      }


      .hero{

        width:94%;

      }


      .features{

        width:94%;

      }


      .hero h1{

        letter-spacing:-1px;

      }


      .btn{

        width:100%;

      }

    }

  </style>

</head>


<body>


  <!-- =========================
       HEADER
  ========================= -->

  <header>

    <div class="navbar">


      <a
        href="#home"
        class="logo">

        <div class="logo-icon">
          🎮
        </div>

        <span>
          AMIR GAMER
        </span>

      </a>


      <button
        class="menu-btn"
        id="menuBtn"
        aria-label="منو">

        ☰

      </button>


      <nav id="mainNav">

        <a href="#home">
          🏠 خانه
        </a>

        <a href="#features">
          ⚡ امکانات
        </a>

        <a href="#news">
          📰 اخبار
        </a>

        <a href="#support">
          📞 پشتیبانی
        </a>

        <a href="#admin">
          🔐 مدیریت
        </a>

      </nav>

    </div>

  </header>


  <!-- =========================
       HERO
  ========================= -->

  <main id="home">

    <section class="hero">


      <div class="hero-content">


        <div class="hero-badge">

          <span>●</span>

          AMIR GAMER ONLINE

        </div>


        <h1>

          <span class="rgb-text">
            AMIR
          </span>

          <br>

          GAMER

        </h1>


        <h2>
          ⚡ دنیای گیمینگ، یک مرحله بالاتر
        </h2>


        <p class="hero-description">

          به سایت رسمی امیر گیمر خوش اومدی.
          اینجا قراره جدیدترین اخبار،
          اطلاعیه‌ها، خدمات و اتفاقات دنیای
          گیمینگ رو در یک محیط خفن و RGB ببینی.

        </p>


        <div class="hero-buttons">

          <a
            href="#news"
            class="btn btn-primary">

            📰 مشاهده اخبار

          </a>


          <a
            href="#support"
            class="btn btn-secondary">

            📞 پشتیبانی

          </a>

        </div>

      </div>


      <!-- VISUAL -->

      <div class="hero-visual">


        <div class="rgb-dot dot1"></div>

        <div class="rgb-dot dot2"></div>

        <div class="rgb-dot dot3"></div>


        <div class="gaming-card">

          <div class="gaming-card-inner">

            <div class="controller">
              🎮
            </div>

            <h3>
              AMIR GAMER
            </h3>

            <p>
              LEVEL UP YOUR GAME
            </p>

          </div>

        </div>

      </div>


    </section>


    <!-- =========================
         FEATURES
    ========================= -->

    <section
      id="features"
      class="features">


      <div class="section-title">

        <span>
          ⚡ امکانات سایت
        </span>

        <p>
          همه‌چیز برای یک تجربه گیمینگ خفن
        </p>

      </div>


      <div class="feature-grid">


        <div class="feature-card">

          <div class="feature-icon">
            📰
          </div>

          <h3>
            اخبار گیمینگ
          </h3>

          <p>
            جدیدترین اخبار و اطلاعیه‌ها
            از طریق پنل مدیریت در سایت
            منتشر می‌شوند.
          </p>

        </div>


        <div class="feature-card">

          <div class="feature-icon">
            ⚡
          </div>

          <h3>
            طراحی RGB
          </h3>

          <p>
            رابط کاربری مدرن با افکت‌های
            RGB و ظاهر مخصوص گیمرها.
          </p>

        </div>


        <div class="feature-card">

          <div class="feature-icon">
            🔐
          </div>

          <h3>
            پنل مدیریت
          </h3>

          <p>
            مدیر سایت می‌تواند اخبار و
            محتوای سایت را مدیریت کند.
          </p>

        </div>


      </div>

    </section>

  </main>


  <!-- =========================
       SUPPORT
  ========================= -->

  <section
    id="support"
    class="features">

    <div class="section-title">

      <span>
        📞 پشتیبانی
      </span>

      <p>
        برای ارتباط با تیم AMIR GAMER
      </p>

    </div>


    <div
      class="feature-grid">


      <div class="feature-card">

        <div class="feature-icon">
          👑
        </div>

        <h3>
          سازنده
        </h3>

        <p>
          آیدی بله:
          <strong style="color:#00eaff">
            @single_Gojo_black_hard
          </strong>
        </p>

      </div>


      <div class="feature-card">

        <div class="feature-icon">
          🛟
        </div>

        <h3>
          پشتیبان دوم
        </h3>

        <p>
          آیدی بله:
          <strong style="color:#ff00cc">
            @fatenehMiri
          </strong>
        </p>

      </div>


      <div class="feature-card">

        <div class="feature-icon">
          📱
        </div>

        <h3>
          شماره پشتیبانی
        </h3>

        <p>
          ۰۹۳۰۳۳۳۲۴۷۶
        </p>

      </div>


    </div>

  </section>


  <!-- =========================
       NEWS PLACEHOLDER
       PART 2 WILL CONNECT HERE
  ========================= -->

  <section
    id="news"
    class="features">

    <div class="section-title">

      <span>
        📰 اخبار
      </span>

      <p>
        اخبار و اطلاعیه‌ها در پارت دوم
        به این بخش متصل می‌شوند.
      </p>

    </div>

    <div
      id="newsContainer"
      class="feature-grid">

      <div class="feature-card">

        <div class="feature-icon">
          📰
        </div>

        <h3>
          به‌زودی...
        </h3>

        <p>
          اخبار سایت از پنل مدیریت
          در این قسمت نمایش داده خواهد شد.
        </p>

      </div>

    </div>

  </section>


  <!-- =========================
       ADMIN PLACEHOLDER
       PART 3 + 4 WILL CONNECT
  ========================= -->

  <section
    id="admin"
    class="features">

    <div class="section-title">

      <span>
        🔐 مدیریت
      </span>

      <p>
        پنل مدیریت در پارت‌های بعدی
        به Firebase متصل می‌شود.
      </p>

    </div>

  </section>


  <!-- =========================
       FOOTER
  ========================= -->

  <footer>

    <div class="footer-inner">

      <div class="footer-copy">

        © 2026
        <span class="footer-brand">
          AMIR GAMER
        </span>

        — تمامی حقوق محفوظ است.

      </div>


      <div class="footer-copy">

        ⚡ GAMING • NEWS • COMMUNITY

      </div>

    </div>

  </footer>


  <!-- =========================
       JAVASCRIPT
  ========================= -->

  <script>

    const menuBtn =
      document.getElementById(
        "menuBtn"
      );

    const mainNav =
      document.getElementById(
        "mainNav"
      );


    menuBtn.addEventListener(
      "click",
      () => {

        mainNav.classList.toggle(
          "active"
        );

      }
    );


    document
      .querySelectorAll(
        "#mainNav a"
      )
      .forEach(
        link => {

          link.addEventListener(
            "click",
            () => {

              mainNav.classList.remove(
                "active"
              );

            }
          );

        }
      );


    /*
      بخش فروش اکانت عمداً در این نسخه
      وجود ندارد.
    */


    console.log(
      "⚡ AMIR GAMER — PART 1 LOADED"
    );

  </script>


</body>

</html>
<!-- پارت دو -->

<style>

/* =========================
   NEWS SECTION
========================= */

#news{

  position:relative;

}


.news-grid{

  display:grid;

  grid-template-columns:
    repeat(3, 1fr);

  gap:20px;

}


.news-card{

  position:relative;

  overflow:hidden;

  border-radius:22px;

  background:
    linear-gradient(
      145deg,
      #ffffff08,
      #ffffff03
    );

  border:
    1px solid #ffffff12;

  transition:
    .35s ease;

}


.news-card:hover{

  transform:
    translateY(-8px);

  border-color:
    #00eaff55;

  box-shadow:
    0 15px 50px #00eaff12;

}


.news-image{

  width:100%;

  height:190px;

  object-fit:cover;

  display:block;

  background:
    linear-gradient(
      135deg,
      #071c28,
      #210b25
    );

}


.news-content{

  padding:22px;

}


.news-tag{

  display:inline-block;

  padding:6px 10px;

  border-radius:20px;

  background:#00eaff0d;

  border:
    1px solid #00eaff25;

  color:#00eaff;

  font-size:11px;

  margin-bottom:12px;

}


.news-title{

  font-size:18px;

  color:#fff;

  line-height:1.7;

  margin-bottom:10px;

}


.news-text{

  color:#888;

  font-size:13px;

  line-height:2;

}


.news-date{

  margin-top:15px;

  color:#555;

  font-size:11px;

}


.news-empty{

  grid-column:
    1 / -1;

  text-align:center;

  padding:50px 20px;

  border:
    1px dashed #ffffff18;

  border-radius:20px;

  color:#777;

}


.news-loading{

  grid-column:
    1 / -1;

  text-align:center;

  padding:40px;

  color:#00eaff;

}


/* =========================
   NEWS MODAL
========================= */

.news-modal{

  position:fixed;

  inset:0;

  z-index:5000;

  display:none;

  align-items:center;

  justify-content:center;

  padding:20px;

  background:
    rgba(0,0,0,.82);

  backdrop-filter:
    blur(12px);

}


.news-modal.active{

  display:flex;

}


.news-modal-box{

  position:relative;

  width:
    min(700px,100%);

  max-height:
    90vh;

  overflow:auto;

  padding:25px;

  border-radius:25px;

  background:
    #090a10;

  border:
    1px solid #ffffff15;

  box-shadow:
    0 0 60px #00eaff15;

}


.news-modal-close{

  position:absolute;

  top:15px;

  left:15px;

  width:38px;

  height:38px;

  border:0;

  border-radius:50%;

  background:#ffffff0d;

  color:#fff;

  font-size:20px;

  cursor:pointer;

}


.news-modal-image{

  width:100%;

  max-height:350px;

  object-fit:cover;

  border-radius:18px;

  margin-bottom:20px;

}


.news-modal h2{

  color:#00eaff;

  font-size:25px;

  line-height:1.7;

  margin-bottom:15px;

}


.news-modal p{

  color:#aaa;

  line-height:2.2;

  white-space:pre-line;

}


/* =========================
   RESPONSIVE
========================= */

@media(max-width:900px){

  .news-grid{

    grid-template-columns:
      repeat(2,1fr);

  }

}


@media(max-width:600px){

  .news-grid{

    grid-template-columns:1fr;

  }


  .news-image{

    height:180px;

  }


  .news-modal-box{

    padding:18px;

  }


  .news-modal h2{

    font-size:20px;

  }

}

</style>


<!-- =========================================================
     NEWS AREA
========================================================= -->

<section
  id="news"
  class="features">


  <div class="section-title">

    <span>
      📰 آخرین اخبار
    </span>

    <p>
      جدیدترین اخبار و اطلاعیه‌های AMIR GAMER
    </p>

  </div>


  <div
    id="newsContainer"
    class="news-grid">


    <div
      class="news-loading">

      ⚡ در حال بارگذاری اخبار...

    </div>


  </div>


</section>


<!-- =========================================================
     NEWS MODAL
========================================================= -->

<div
  id="newsModal"
  class="news-modal">


  <div class="news-modal-box">


    <button
      id="newsModalClose"
      class="news-modal-close">

      ×

    </button>


    <img
      id="newsModalImage"
      class="news-modal-image"
      alt="خبر">


    <h2
      id="newsModalTitle">
    </h2>


    <p
      id="newsModalText">
    </p>


    <div
      id="newsModalDate"
      class="news-date">
    </div>


  </div>

</div>


<script>

/* =========================================================
   NEWS DATA
   فعلاً از LocalStorage استفاده می‌کنیم.
   در پارت ۴ به Firebase متصل می‌شود.
========================================================= */


const AMIR_GAMER_NEWS_KEY =
  "amir_gamer_news";


/* =========================================================
   DEFAULT NEWS
========================================================= */

function getDefaultNews(){

  return [

    {

      id:
        "welcome-1",

      title:
        "🎮 به AMIR GAMER خوش آمدید",

      text:
        "به سایت رسمی AMIR GAMER خوش آمدید. از این قسمت جدیدترین اخبار، اطلاعیه‌ها و اتفاقات گیمینگ را دنبال کنید.",

      image:
        "",

      date:
        "اخبار سایت"

    },

    {

      id:
        "support-1",

      title:
        "📢 راه‌های ارتباط با پشتیبانی",

      text:
        "برای ارتباط با تیم AMIR GAMER می‌توانید از آیدی‌های پشتیبانی در بله استفاده کنید.",

      image:
        "",

      date:
        "اطلاعیه"

    }

  ];

}


/* =========================================================
   GET NEWS
========================================================= */

function getNews(){

  try{

    const saved =
      localStorage.getItem(
        AMIR_GAMER_NEWS_KEY
      );


    if(saved){

      const parsed =
        JSON.parse(saved);


      if(
        Array.isArray(parsed)
      ){

        return parsed;

      }

    }

  }catch(error){

    console.error(
      "NEWS LOAD ERROR:",
      error
    );

  }


  const defaults =
    getDefaultNews();


  localStorage.setItem(

    AMIR_GAMER_NEWS_KEY,

    JSON.stringify(
      defaults
    )

  );


  return defaults;

}


/* =========================================================
   SAVE NEWS
========================================================= */

function saveNews(news){

  localStorage.setItem(

    AMIR_GAMER_NEWS_KEY,

    JSON.stringify(
      news
    )

  );

}


/* =========================================================
   ESCAPE HTML
========================================================= */

function escapeNewsHTML(text){

  if(text === null ||
     text === undefined){

    return "";

  }


  return String(text)

    .replace(
      /&/g,
      "&amp;"
    )

    .replace(
      /</g,
      "&lt;"
    )

    .replace(
      />/g,
      "&gt;"
    )

    .replace(
      /"/g,
      "&quot;"
    )

    .replace(
      /'/g,
      "&#039;"
    );

}


/* =========================================================
   RENDER NEWS
========================================================= */

function renderNews(){

  const container =
    document.getElementById(
      "newsContainer"
    );


  if(!container){

    return;

  }


  const news =
    getNews();


  container.innerHTML =
    "";


  if(
    !news ||
    news.length === 0
  ){

    container.innerHTML = `

      <div class="news-empty">

        📰

        <br><br>

        هنوز خبری منتشر نشده است.

      </div>

    `;

    return;

  }


  news.forEach(
    item => {


      const title =
        escapeNewsHTML(
          item.title
        );


      const text =
        escapeNewsHTML(
          item.text
        );


      const date =
        escapeNewsHTML(
          item.date ||
          "AMIR GAMER"
        );


      let imageHTML = "";


      if(item.image){

        imageHTML = `

          <img
            class="news-image"
            src="${escapeNewsHTML(item.image)}"
            alt="${title}"
            onerror="
              this.style.display='none'
            ">

        `;

      }else{

        imageHTML = `

          <div
            class="news-image"
            style="
              display:flex;
              align-items:center;
              justify-content:center;
              font-size:65px;
            ">

            🎮

          </div>

        `;

      }


      container.innerHTML += `

        <article
          class="news-card">


          ${imageHTML}


          <div
            class="news-content">


            <span
              class="news-tag">

              ⚡ AMIR GAMER

            </span>


            <h3
              class="news-title">

              ${title}

            </h3>


            <p
              class="news-text">

              ${text.substring(0,180)}

              ${text.length > 180 ? "..." : ""}

            </p>


            <div
              class="news-date">

              📅 ${date}

            </div>


            <button
              class="btn btn-secondary"
              style="
                width:100%;
                margin-top:15px;
                cursor:pointer;
                border:1px solid #00eaff25;
                background:#00eaff08;
              "
              onclick="
                openNews(
                  '${escapeNewsHTML(item.id)}'
                )
              ">

              👁️ مشاهده کامل خبر

            </button>


          </div>


        </article>

      `;

    }
  );

}


/* =========================================================
   OPEN NEWS
========================================================= */

function openNews(id){

  const news =
    getNews();


  const item =
    news.find(
      x =>
        String(x.id) ===
        String(id)
    );


  if(!item){

    return;

  }


  const modal =
    document.getElementById(
      "newsModal"
    );


  const image =
    document.getElementById(
      "newsModalImage"
    );


  const title =
    document.getElementById(
      "newsModalTitle"
    );


  const text =
    document.getElementById(
      "newsModalText"
    );


  const date =
    document.getElementById(
      "newsModalDate"
    );


  title.textContent =
    item.title || "";


  text.textContent =
    item.text || "";


  date.textContent =
    "📅 " +
    (
      item.date ||
      "AMIR GAMER"
    );


  if(item.image){

    image.src =
      item.image;

    image.style.display =
      "block";

  }else{

    image.style.display =
      "none";

  }


  modal.classList.add(
    "active"
  );


  document.body.style.overflow =
    "hidden";

}


/* =========================================================
   CLOSE NEWS
========================================================= */

function closeNews(){

  const modal =
    document.getElementById(
      "newsModal"
    );


  modal.classList.remove(
    "active"
  );


  document.body.style.overflow =
    "";

}


document
  .getElementById(
    "newsModalClose"
  )
  .addEventListener(
    "click",
    closeNews
  );


document
  .getElementById(
    "newsModal"
  )
  .addEventListener(
    "click",
    event => {

      if(
        event.target.id ===
        "newsModal"
      ){

        closeNews();

      }

    }
  );


document.addEventListener(
  "keydown",
  event => {

    if(
      event.key ===
      "Escape"
    ){

      closeNews();

    }

  }
);


/* =========================================================
   INITIALIZE
========================================================= */

document.addEventListener(
  "DOMContentLoaded",
  () => {

    renderNews();

  }
);


/* =========================================================
   ADMIN HELPER FUNCTIONS
   پارت ۳ از این توابع استفاده می‌کند.
========================================================= */

window.AMIR_GAMER_NEWS = {

  get:
    getNews,

  save:
    saveNews,

  render:
    renderNews,

  open:
    openNews,

  close:
    closeNews

};


console.log(
  "📰 AMIR GAMER — PART 2 LOADED"
);

</script>
<!-- پارت سه-->

<style>

/* =========================
   ADMIN
========================= */

.admin-section{

  width:92%;

  max-width:1250px;

  margin:0 auto;

  padding:60px 0 100px;

}


.admin-login-box{

  max-width:450px;

  margin:auto;

  padding:30px;

  border-radius:24px;

  background:#ffffff06;

  border:1px solid #ffffff14;

  box-shadow:
    0 0 40px #00eaff08;

}


.admin-login-icon{

  width:70px;

  height:70px;

  margin:0 auto 18px;

  display:flex;

  align-items:center;

  justify-content:center;

  border-radius:20px;

  font-size:32px;

  background:
    linear-gradient(
      135deg,
      #00eaff20,
      #ff00cc20
    );

  border:
    1px solid #ffffff15;

}


.admin-login-box h2{

  text-align:center;

  color:#00eaff;

  margin-bottom:8px;

}


.admin-login-box p{

  text-align:center;

  color:#777;

  font-size:13px;

  margin-bottom:25px;

}


.admin-input{

  width:100%;

  padding:14px;

  margin-bottom:14px;

  border-radius:12px;

  border:1px solid #ffffff15;

  outline:none;

  background:#050509;

  color:#fff;

  font-family:inherit;

}


.admin-input:focus{

  border-color:#00eaff;

  box-shadow:
    0 0 15px #00eaff10;

}


.admin-login-button{

  width:100%;

  padding:14px;

  border:0;

  border-radius:12px;

  cursor:pointer;

  color:#fff;

  font-weight:bold;

  font-family:inherit;

  background:
    linear-gradient(
      90deg,
      #00eaff,
      #7b2cff,
      #ff00cc
    );

  background-size:200%;

  transition:.3s;

}


.admin-login-button:hover{

  background-position:100%;

  transform:
    translateY(-2px);

}


/* =========================
   DASHBOARD
========================= */

.admin-dashboard{

  display:none;

}


.admin-dashboard.active{

  display:block;

}


.admin-header{

  display:flex;

  align-items:center;

  justify-content:space-between;

  gap:20px;

  padding:22px;

  margin-bottom:20px;

  border-radius:20px;

  background:#ffffff06;

  border:1px solid #ffffff12;

}


.admin-header h2{

  color:#00eaff;

  margin-bottom:7px;

}


.admin-header p{

  color:#777;

  font-size:12px;

}


.admin-logout{

  padding:11px 17px;

  border-radius:10px;

  border:
    1px solid #ff174433;

  background:#ff174410;

  color:#ff5370;

  cursor:pointer;

  font-family:inherit;

}


/* =========================
   TABS
========================= */

.admin-tabs{

  display:flex;

  flex-wrap:wrap;

  gap:10px;

  margin-bottom:20px;

}


.admin-tab{

  padding:11px 18px;

  border-radius:11px;

  border:1px solid #ffffff12;

  background:#ffffff06;

  color:#888;

  cursor:pointer;

  font-family:inherit;

}


.admin-tab.active{

  color:#fff;

  border-color:#00eaff55;

  background:#00eaff0d;

}


/* =========================
   ADMIN PANELS
========================= */

.admin-panel{

  display:none;

  padding:25px;

  border-radius:20px;

  background:#ffffff05;

  border:1px solid #ffffff12;

}


.admin-panel.active{

  display:block;

}


.admin-panel-title{

  color:#fff;

  margin-bottom:20px;

  font-size:20px;

}


.admin-form{

  display:grid;

  gap:14px;

}


.admin-form textarea{

  min-height:160px;

  resize:vertical;

}


.admin-form-actions{

  display:flex;

  flex-wrap:wrap;

  gap:10px;

}


.admin-save{

  flex:1;

  min-width:150px;

  padding:13px;

  border:0;

  border-radius:11px;

  background:
    linear-gradient(
      90deg,
      #00eaff,
      #7b2cff
    );

  color:#fff;

  cursor:pointer;

  font-family:inherit;

  font-weight:bold;

}


.admin-clear{

  flex:1;

  min-width:150px;

  padding:13px;

  border-radius:11px;

  border:1px solid #ffffff15;

  background:#ffffff07;

  color:#aaa;

  cursor:pointer;

  font-family:inherit;

}


/* =========================
   NEWS ADMIN LIST
========================= */

.admin-news-list{

  display:grid;

  gap:14px;

  margin-top:25px;

}


.admin-news-item{

  display:flex;

  align-items:center;

  justify-content:space-between;

  gap:20px;

  padding:18px;

  border-radius:15px;

  background:#050509;

  border:1px solid #ffffff10;

}


.admin-news-info{

  min-width:0;

}


.admin-news-info h4{

  color:#00eaff;

  margin-bottom:8px;

}


.admin-news-info p{

  color:#777;

  font-size:12px;

  overflow:hidden;

  text-overflow:ellipsis;

}


.admin-news-actions{

  display:flex;

  flex-wrap:wrap;

  gap:7px;

}


.admin-small-btn{

  padding:8px 11px;

  border:0;

  border-radius:8px;

  cursor:pointer;

  color:#fff;

  font-family:inherit;

}


.admin-edit{

  background:#1769aa;

}


.admin-delete{

  background:#941c3a;

}


/* =========================
   STATUS
========================= */

.admin-status{

  display:none;

  padding:12px;

  margin-bottom:15px;

  border-radius:10px;

  background:#00eaff08;

  border:1px solid #00eaff20;

  color:#00eaff;

  font-size:13px;

}


.admin-status.show{

  display:block;

}


/* =========================
   SECURITY NOTICE
========================= */

.admin-security{

  margin-top:20px;

  padding:15px;

  border-radius:12px;

  background:#ffb30008;

  border:1px solid #ffb30020;

  color:#c99b3b;

  font-size:12px;

  line-height:1.9;

}


/* =========================
   RESPONSIVE
========================= */

@media(max-width:700px){

  .admin-header{

    flex-direction:column;

    align-items:stretch;

  }


  .admin-news-item{

    flex-direction:column;

    align-items:stretch;

  }


  .admin-news-actions{

    width:100%;

  }


  .admin-small-btn{

    flex:1;

  }

}

</style>


<!-- =========================================================
     ADMIN SECTION
========================================================= -->

<section
  id="admin"
  class="admin-section">


  <!-- =========================
       LOGIN
  ========================= -->

  <div
    id="adminLoginBox"
    class="admin-login-box">


    <div class="admin-login-icon">
      🔐
    </div>


    <h2>
      پنل مدیریت AMIR GAMER
    </h2>


    <p>
      فقط مدیر سایت می‌تواند وارد این بخش شود.
    </p>


    <input
      id="adminUsername"
      class="admin-input"
      type="text"
      autocomplete="username"
      placeholder="نام کاربری">


    <input
      id="adminPassword"
      class="admin-input"
      type="password"
      autocomplete="current-password"
      placeholder="رمز عبور">


    <button
      id="adminLoginButton"
      class="admin-login-button"
      type="button">

      🔑 ورود به پنل

    </button>


    <div
      class="admin-security">

      🔒 در نسخه نهایی، احراز هویت واقعی
      با Firebase انجام می‌شود و رمز عبور
      داخل فایل HTML ذخیره نخواهد شد.

    </div>


  </div>


  <!-- =========================
       DASHBOARD
  ========================= -->

  <div
    id="adminDashboard"
    class="admin-dashboard">


    <div class="admin-header">


      <div>

        <h2>
          ⚡ AMIR GAMER ADMIN
        </h2>

        <p>
          مدیریت اخبار و محتوای سایت
        </p>

      </div>


      <button
        id="adminLogout"
        class="admin-logout">

        🚪 خروج

      </button>


    </div>


    <!-- STATUS -->

    <div
      id="adminStatus"
      class="admin-status">
    </div>


    <!-- TABS -->

    <div class="admin-tabs">


      <button
        class="admin-tab active"
        data-panel="newsManager">

        📰 مدیریت اخبار

      </button>


      <button
        class="admin-tab"
        data-panel="siteInfo">

        ⚙️ اطلاعات سایت

      </button>


      <button
        class="admin-tab"
        data-panel="supportInfo">

        📞 پشتیبانی

      </button>


    </div>


    <!-- =========================
         NEWS MANAGER
    ========================= -->

    <div
      id="newsManager"
      class="admin-panel active">


      <h3 class="admin-panel-title">
        📰 افزودن / ویرایش خبر
      </h3>


      <form
        id="adminNewsForm"
        class="admin-form">


        <input
          id="adminNewsId"
          type="hidden">


        <input
          id="adminNewsTitle"
          class="admin-input"
          type="text"
          placeholder="عنوان خبر"
          required>


        <input
          id="adminNewsImage"
          class="admin-input"
          type="url"
          placeholder="لینک تصویر خبر (اختیاری)">


        <input
          id="adminNewsDate"
          class="admin-input"
          type="text"
          placeholder="تاریخ یا برچسب خبر">


        <textarea
          id="adminNewsText"
          class="admin-input"
          placeholder="متن کامل خبر"
          required>
        </textarea>


        <div
          class="admin-form-actions">


          <button
            class="admin-save"
            type="submit">

            💾 ذخیره خبر

          </button>


          <button
            id="adminClearNews"
            class="admin-clear"
            type="button">

            🧹 پاک کردن فرم

          </button>


        </div>


      </form>


      <div
        id="adminNewsList"
        class="admin-news-list">
      </div>


    </div>


    <!-- =========================
         SITE INFO
    ========================= -->

    <div
      id="siteInfo"
      class="admin-panel">


      <h3 class="admin-panel-title">
        ⚙️ اطلاعات سایت
      </h3>


      <form
        id="siteInfoForm"
        class="admin-form">


        <input
          id="siteName"
          class="admin-input"
          type="text"
          value="AMIR GAMER"
          placeholder="نام سایت">


        <textarea
          id="siteDescription"
          class="admin-input"
          placeholder="توضیحات سایت">به سایت رسمی AMIR GAMER خوش آمدید.</textarea>


        <button
          class="admin-save"
          type="submit">

          💾 ذخیره اطلاعات

        </button>


      </form>


    </div>


    <!-- =========================
         SUPPORT INFO
    ========================= -->

    <div
      id="supportInfo"
      class="admin-panel">


      <h3 class="admin-panel-title">
        📞 اطلاعات پشتیبانی
      </h3>


      <form
        id="supportInfoForm"
        class="admin-form">


        <input
          id="supportCreator"
          class="admin-input"
          type="text"
          value="@single_Gojo_black_hard"
          placeholder="آیدی سازنده در بله">


        <input
          id="supportSecond"
          class="admin-input"
          type="text"
          value="@fatenehMiri"
          placeholder="آیدی پشتیبان دوم در بله">


        <input
          id="supportPhone"
          class="admin-input"
          type="text"
          value="۰۹۳۰۳۳۳۲۴۷۶"
          placeholder="شماره پشتیبانی">


        <button
          class="admin-save"
          type="submit">

          💾 ذخیره پشتیبانی

        </button>


      </form>


    </div>


  </div>


</section>


<script>

/* =========================================================
   ADMIN LOCAL SYSTEM
   در پارت ۴ احراز هویت Firebase جایگزین این قسمت می‌شود.
========================================================= */


/*
   این اطلاعات فقط برای تست ظاهری پارت ۳ هستند.
   
   برای سایت واقعی نباید رمز مدیریت را
   داخل فایل JavaScript قرار دهیم.
*/

const ADMIN_TEST_USERNAME =
  "admin";

const ADMIN_TEST_PASSWORD =
  "AmirGamer@2026";


/* =========================================================
   ELEMENTS
========================================================= */

const adminLoginBox =
  document.getElementById(
    "adminLoginBox"
  );


const adminDashboard =
  document.getElementById(
    "adminDashboard"
  );


const adminUsername =
  document.getElementById(
    "adminUsername"
  );


const adminPassword =
  document.getElementById(
    "adminPassword"
  );


const adminLoginButton =
  document.getElementById(
    "adminLoginButton"
  );


const adminLogout =
  document.getElementById(
    "adminLogout"
  );


const adminStatus =
  document.getElementById(
    "adminStatus"
  );


/* =========================================================
   STATUS MESSAGE
========================================================= */

function showAdminStatus(
  message
){

  adminStatus.textContent =
    message;

  adminStatus.classList.add(
    "show"
  );


  setTimeout(
    () => {

      adminStatus.classList.remove(
        "show"
      );

    },
    3000
  );

}


/* =========================================================
   LOGIN
========================================================= */

adminLoginButton.addEventListener(
  "click",
  () => {


    const username =
      adminUsername
        .value
        .trim();


    const password =
      adminPassword
        .value;


    if(
      username ===
        ADMIN_TEST_USERNAME
      &&
      password ===
        ADMIN_TEST_PASSWORD
    ){

      sessionStorage.setItem(
        "amir_gamer_admin",
        "true"
      );


      adminLoginBox.style.display =
        "none";


      adminDashboard.classList.add(
        "active"
      );


      loadAdminNews();


      showAdminStatus(
        "✅ ورود موفق بود."
      );


    }else{

      showAdminStatus(
        "❌ نام کاربری یا رمز عبور اشتباه است."
      );

    }

  }
);


/* =========================================================
   ENTER KEY LOGIN
========================================================= */

adminPassword.addEventListener(
  "keydown",
  event => {

    if(
      event.key ===
      "Enter"
    ){

      adminLoginButton.click();

    }

  }
);


/* =========================================================
   LOGOUT
========================================================= */

adminLogout.addEventListener(
  "click",
  () => {

    sessionStorage.removeItem(
      "amir_gamer_admin"
    );


    adminDashboard.classList.remove(
      "active"
    );


    adminLoginBox.style.display =
      "block";


    adminUsername.value =
      "";


    adminPassword.value =
      "";


    showAdminStatus(
      "🚪 از پنل خارج شدی."
    );

  }
);


/* =========================================================
   RESTORE SESSION
========================================================= */

function restoreAdmin(){

  const loggedIn =
    sessionStorage.getItem(
      "amir_gamer_admin"
    );


  if(
    loggedIn ===
    "true"
  ){

    adminLoginBox.style.display =
      "none";


    adminDashboard.classList.add(
      "active"
    );


    loadAdminNews();

  }

}


restoreAdmin();


/* =========================================================
   TABS
========================================================= */

document
  .querySelectorAll(
    ".admin-tab"
  )
  .forEach(
    tab => {

      tab.addEventListener(
        "click",
        () => {


          document
            .querySelectorAll(
              ".admin-tab"
            )
            .forEach(
              item => {

                item.classList.remove(
                  "active"
                );

              }
            );


          document
            .querySelectorAll(
              ".admin-panel"
            )
            .forEach(
              panel => {

                panel.classList.remove(
                  "active"
                );

              }
            );


          tab.classList.add(
            "active"
          );


          const panel =
            document.getElementById(
              tab.dataset.panel
            );


          if(panel){

            panel.classList.add(
              "active"
            );

          }

        }
      );

    }
  );


/* =========================================================
   NEWS ADMIN
========================================================= */

function loadAdminNews(){

  const list =
    document.getElementById(
      "adminNewsList"
    );


  if(!list){

    return;

  }


  const news =
    window.AMIR_GAMER_NEWS
      ? window.AMIR_GAMER_NEWS.get()
      : [];


  list.innerHTML =
    "";


  if(
    news.length ===
    0
  ){

    list.innerHTML = `

      <div class="news-empty">

        📰 خبری ثبت نشده است.

      </div>

    `;

    return;

  }


  news.forEach(
    item => {


      const div =
        document.createElement(
          "div"
        );


      div.className =
        "admin-news-item";


      div.innerHTML = `

        <div
          class="admin-news-info">

          <h4></h4>

          <p></p>

        </div>


        <div
          class="admin-news-actions">


          <button
            class="admin-small-btn admin-edit"
            type="button">

            ✏️ ویرایش

          </button>


          <button
            class="admin-small-btn admin-delete"
            type="button">

            🗑️ حذف

          </button>


        </div>

      `;


      div
        .querySelector("h4")
        .textContent =
          item.title || "";


      div
        .querySelector("p")
        .textContent =
          item.text || "";


      div
        .querySelector(".admin-edit")
        .addEventListener(
          "click",
          () => {

            editAdminNews(
              item.id
            );

          }
        );


     
