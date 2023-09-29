
<html>
  <head>
    <meta charset="utf-8" />
    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>WEB PERTAMA</title>
    <style>
      *,
      html,
      body {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Helvetica;
        scroll-behavior: smooth;
      }

      header {
        background: #1a2238;
        color: #eaeaea;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 10px;
      }

      .logo {
        margin-right: auto;
        display: flex;
        gap: 6px;
      }

      .logo-img {
        width: 35px;
        height: 35px;
        margin-left: 10px;
      }

      .logo-title {
        cursor: pointer;
        transition: all 0.5s ease 0s;
      }

      .logo:hover {
        color: #ff6a3d;
        transform: rotate(2deg);
      }

      .button {
        display: inline-block;
        padding: 10px 20px;
        font-size: 16px;
        font-weight: bold;
        text-align: center;
        text-decoration: none;
        border-radius: 7px;
        transition: background-color 0.5s ease;
        margin-right: 10px;
      }

      .button-elegant {
        background-color: #e8e8e8;
        color: #333;
        border: 2px solid #e8e8e8;
      }

      .button-elegant:hover {
        background-color: #333;
        color: #fff;
        border: 2px solid #333;
      }

      .button-elegant:active {
        background-color: #555;
        color: #fff;
        border: 2px solid #555;
      }

      li {
        list-style-type: none;
        padding: 10px;
      }

      nav ul {
        display: flex;
        list-style: none;
        align-items: center;
        padding: 20px;
      }
      nav ul li a {
        text-decoration: none;
        font-family: "Segoe UI", sans-serif;
        color: white;
        font-weight: 600;
        padding: 8px 2px;
        transition: all 5s ease 0s;
        transition-duration: 300ms;
        border-bottom: 1px solid rgba(255, 68, 0, 0);
        display: inline-block;
      }
      nav ul li a:hover {
        border-bottom: 1px solid white;
        color: skyblue;
        transform: rotate(2deg);
      }

      .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 70px 0;
      }

      .intro {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
        text-align: center;
      }

      .title {
        font-size: 24px;
        font-weight: bold;
      }

      .description {
        font-size: 28px;
        font-weight: bolder;
      }

      .img-foto {
        width: 100%;
        height: auto;
        padding: 10px;
        max-width: 500px;
      }

      .parallax {
        background-image: url("assets/foto/semismile.png");
        background-attachment: fixed;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 100vh;
      }

      .tentang {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        background: #1a2238;
        color: #eaeaea;
        padding: 40px;
      }

      .mt-10 {
        margin-top: 20px;
      }

      .card {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 8px;
      }

      .card-item {
        text-align: center;
        width: 25%;
        min-height: 200px;
        max-height: 300px;
        background: #f7f7f7;
        color: #222;
        padding: 24px;
        box-shadow: 2px 5px 5px 1px rgba(0, 0, 0, 0.5);
      }

      .card-title {
        font-size: 18px;
        font-weight: bolder;
      }

      .card-description {
        font-size: 14px;
        margin-top: 4px;
      }

      .icon {
        width: 75px;
        height: 75px;
        margin: 10px;
        padding: 4px;
      }

      footer {
        padding: 20px;
        text-align: center;
        background: #1a2238;
        color: #eaeaea;
      }

      @media screen and (max-width: 410px) {
        .card {
          flex-direction: column;
          gap: 0;
        }
        .card-item {
          width: 100%;
          opacity: 0.9;
        }

        .container {
          width: 100%;
          padding: 0;
        }

        .intro {
          margin-top: 20px;
        }

        .img-foto {
          padding: 0;
        }

        nav {
          position: fixed;
          bottom: 0;
          width: 100%;
          background: #1a2238;
          z-index: 9;
        }

        footer {
          margin-bottom: 70px;
          margin-top: 70px;
        }
      }
    </style>
  </head>
  <body>
    <header>
      <div class="logo">
        <img src="arel.jpg" alt="" class="logo-img" />
        <h1 class="logo-title">HYDRA</h1>
      </div>

      <nav>
        <ul>
          <li><a href="#jasa">Home</a></li>
          <li><a href="mailto:deacode@icloud.com">Lab</a></li>
          <li><a href="">About</a></li>
        </ul>
      </nav>
      <button class="button button-elegant" onclick="redirInstagram()">
        Follow
      </button>
    </header>
    <div class="container">
      <div class="intro">
        <p class="title">Hello, Gabriel Wahyu Handrajati Here!</p>
        <p class="description">Faculty informatics of engineering UAJY.</p>
        <img src="arel.jpg" alt="" class="img-foto" />
      </div>
    </div>
    <div class="parallax">
      <div class="tentang">
        <p class="title">Saya Adalah Web Development</p>
        <p class="description">Hajar ae lahh boss, jagonya belakangan.</p>
        <div class="mt-10">
          <button class="button button-elegant" onclick="redirWhatsapp()">
            Kontak
          </button>
        </div>
      </div>
      <div class="container">
        <div class="card" id="jasa">
          <div class="card-item">
            <img src="arelckgrndnone.jpg" alt="" class="icon" />
            <p class="card-title">Profile</p>
            <p class="card-description">Hai kenalin gw Gabriel</p>
          </div>
          <div class="card-item">
            <img src="logouajy.jpg" alt="" class="icon" />
            <p class="card-title">My University</p>
            <p class="card-description">Universitas Atma Jaya Yogyakarta</p>
          </div>
          <div class="card-item">
            <img src="fti.jpg" alt="" class="icon" />
            <p class="card-title">Faculty</p>
            <p class="card-description">Fakultas Teknologi Industri</p>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <p class="title">&copy; GabrielWahyuWebsite2022</p>
    </footer>

    <script>
      function redirInstagram() {
        window.location.href = "https://instagram.com/cibonara._";
      }

      function redirWhatsapp() {
        window.location.href = "";
      }
    </script>
  </body>
</html>
