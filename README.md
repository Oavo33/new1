<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Hub</title>
  <style>@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');
    body {
      font-family: 'Roboto', sans-serif;
      font-size: 14px;
      background-color: #f2f2f2;
      color: #333333;
      margin: 0;
      padding: 0;
    }
    header {
      background: linear-gradient(to bottom, #00b3b3, #008080);
      padding: 40px 20px;
      text-align: center;
      position: relative;
    }
    header .hub-title {
      font-size: 38px;
    }
    header h1 {
      font-size: 38px;
      color: #ffffff;
      margin: 0;
    }
    .social {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
    }
    .social div {
      margin-bottom: 5px;
    }
    .social div a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: black;
    }
    .social div a img {
      width: 15px;
      height: 15px;
    }
    .login {
      position: absolute;
      top: 14px;
      right: 14px;
      display: flex;
      align-items: center;
      font-weight: bold;
      text-decoration: none;
    }
    .login a {
      color: yellow !important;
    }
    .login:hover .tooltip {
      visibility: visible;
      opacity: 1;
    }
    .tooltip {
      position: absolute;
      top: 75%;
      right: 35%;
      width: 200px;
      background-color: #f9f9f9;
      border: 1px solid #ccc;
      border-radius: 5px;
      padding: 10px;
      font-size: 14px;
      color: black;
      text-align: center;
      visibility: hidden;
      opacity: 5;
      transition: visibility 0s, opacity 0.3s ease-in-out;
    }
    .hub-card {
      background: linear-gradient(to bottom, #008080, #00b3b3);
      border-radius: 10px;
      border: 2px solid #ffffff;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      padding: 10px;
      text-align: center;
      max-width: 210px;
      width: 45%;
      margin: 0 auto;
      margin-top: -136px;
      position: relative;
      z-index: 2;
    }
    .hub-card h1 {
      font-size: 16px;
      margin-top: 0;
      margin-bottom: 2px;
      color: #ffffff;
    }
    .hub-card p {
      font-size: 14px;
      margin-bottom: 2px;
      color: #ffffff;
    }
    .graffiti {
      position: absolute;
      transform: translate(-50%, -50%);
      font-family: 'Roboto', sans-serif;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
      z-index: 1;
      left: 2px;
      font-size: 10px;
      transform: rotate(-7deg);
      top: 2%;
      color: white;
    }
    .box {
      display: inline-block;
      padding: 1px;
      border: 1px solid #E53E3E;
      background-color: transparent;
      border-radius: 4px;
    }
    .box a {
      color: white;
      text-decoration: none;
      padding: 8px 16px;
      background-color: #E53E3E;
      border-radius: 4px;
      transition: background-color 0.3s ease-in-out;
    }
    .box a:hover {
      background-color: #ff4c4c;
    }
    .grid-wrapper {
      display: flex;
      justify-content: center;
    }
    .grid-container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-gap: 20px;
      max-width: 90%;
      margin-top: 20px;
      margin-bottom: 20px;
      margin-left: auto;
      margin-right: auto;
    }
    .grid-container .grid-item {
      background-color: #00b3b3;
      color: #ffffff;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2), 0 6px 6px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s, box-shadow 0.3s;
      cursor: pointer;
      font-size: 14px;
      padding: 10px;
      text-align: center;
    }
    .grid-container .grid-item:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3), 0 8px 8px rgba(0, 0, 0, 0.3);
    }
    .grid-container .grid-item .hover-text {
      display: none;
      font-size: 10px;
    }
    .grid-container .grid-item:hover .hover-text {
      display: block;
    }footer {
      background: linear-gradient(to bottom, #ffffff, #00b3b3);
      padding: 35px;
      color: #ffffff;
      text-align: center;
      font-size: 14px;
    }
    .footer-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
    }
    .footer-container .box {
      background-color: #00b3b3;
      color: #ffffff;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2), 0 6px 6px rgba(0, 0, 0, 0.2);
      padding: 10px;
      text-align: center;
      margin: 10px;
      cursor: pointer;
    }
    .footer-container .box h3 {
      margin: 0;
    }
    .footer-container .box:first-child {
      border: 1px solid #ffffff;
    }
    .footer-container .box:last-child {
      border: 1px solid #ffffff;
    }
  </style>
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-RZG8MP5HRX"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-RZG8MP5HRX');
  </script>
</head>
<body>
<header>
  <div class="graffiti">
    This is your Hub !<br>
    Do you want to change It ?<br>
    Submit Request <br>
    <span class="box"><button class="custom-class" onclick="window.open('https://docs.google.com/forms/d/e/1FAIpQLScrHwrJjCwCha1DkU4ZNGvWP2zR41vlqTsyVuK-prMGZjFgQQ/viewform?embedded=true')">Here</button></span>
  </div>
  <div class="login">
    <button class="custom-class">Login</button>
    <div class="tooltip">
      You don't need to Sign Up! You are already a Member of Our Community. Save that time browsing what's on offer this week!
    </div>
  </div>
  <h1 class="hub-title">HubBook</h1>
  <div class="social">
    <div>
      <button class="custom-class" onclick="window.open('#')">
        <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
      </button>
    </div>
    <div>
      <button class="custom-class" onclick="window.open('#')">
        <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
      </button>
    </div>
    <div>
      <button class="custom-class" onclick="window.open('#')">
        <img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram">
      </button>
    </div>
    <div>
      <button class="custom-class" onclick="window.open('#')">
        <img src="https://img.icons8.com/office/30/FF0000/twitter.png" alt="Twitter">
      </button>
    </div>
  </div>
</header>
<div class="hub-card">
  <h1>Message From The Team</h1>
  <p>Hi There, At The Hub We Have A Team Of Your Local Community Members Who Have Built This Hub For You! To Help Local Community And Local Business Get Together And Share Each Other's Skills!</p>
</div>
<div class="grid-container">
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/Elderly.assistance/')">
      <i class="community-icon">👵👴🏽</i>
      <p class="community-text">Elderly Assistance</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/Personalized.Exchange.And.Free.Services/')">
      <i class="community-icon">🤝</i>
      <p class="community-text">Community Giveaway</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/The.Community.Graffiti.Wall')">
      <i class="community-icon">🎨</i>
      <p class="community-text">The Community Graffiti Wall</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/Vintage.High.Street/')">
      <i class="community-icon">📸</i>
      <p class="community-text">Our Vintage Shop Memories</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/Help/')">
      <i class="community-icon">🏠</i>
      <p class="community-text">Help Our Homeless</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/The.Hub/')">
      <i class="community-icon">💼</i>
      <p class="community-text">Encouraging Young Entrepreneurship</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/Personalized.Web.Pages/')">
      <i class="community-icon">🌐</i>
      <p class="community-text">FREE Web Pages, Every Month</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('https://oavo33.github.io/White.Paper/')">
      <i class="community-icon">📝</i>
      <p class="community-text">White Paper</p>
    </button>
  </div>
  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🌟</i>
      <p class="community-text">New Button 1</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🎯</i>
      <p class="community-text">New Button 2</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🎮</i>
      <p class="community-text">New Button 3</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🌺</i>
      <p class="community-text">New Button 4</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🍕</i>
      <p class="community-text">New Button 5</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">📚</i>
      <p class="community-text">New Button 6</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">⚽</i>
      <p class="community-text">New Button 7</p>
      <p class="community-text">New Button 8</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🎨</i>
      <p class="community-text">New Button 8</p>
      <p class="community-text">New Button 8</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🎧</i>
      <p class="community-text">New Button 9</p>
    </button>
  </div>

  <div class="grid-item">
    <button class="custom-class" onclick="window.open('URL_HERE')">
      <i class="community-icon">🌈</i>
      <p class="community-text">New Button 10</p>
    </button>
  </div></div>
<footer>
  <div class="footer-container">
    <div class="box">
      <h3>Contact</h3>
      <p>Email: contact@thehub.com</p>
      <p>Phone: 123-456-7890</p>
    </div>
    <div class="box">
      <h3>About Us</h3>
      <h3>Terms of Service</h3>
      <p>By using The Hub, you agree to our Terms of Service and Privacy Policy. Please read them carefully before accessing or using our platform.</p>
    </div>
  </div>
  <footer>
    <div class="footer-container">
      <div class="box" onclick="window.location.href = 'https://oavo33.github.io/GitHubz/';">
        <h3>What Do You Think About Our Community Hub?</h3>
      </div>
      <div class="box" onclick="scrollToTop()">🚀</div>
    </div>
    <div class="footer-container">
      <p>&copy; 2023 Lofties. All rights reserved.</p>
    </div>
  </footer>
<script>
  function showMenu(element) {
    var menu = element.querySelector(".hover-menu");
    menu.style.display = "block";
  }</script>
</body>
</html>
