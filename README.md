<!DOCTYPE html><html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Hub</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');
    body {
      font-family: 'Space Mono', monospace;
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
    }.graffiti {
      position: absolute;
      transform: translate(-50%, -50%);
      font-family: 'Space Mono', monospace;
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
    }
    .box a {
      color: white;
      text-decoration: none;
    }
    .grid-wrapper {
      overflow-x: scroll;
    }
    .grid-container {
      width: 140%;
    }
    .grid-container .grid-item {
      cursor: pointer;
      text-align: center;
      background-color: #f2f2f2;
      border-radius: 5px;
      padding: 20px;
      margin-bottom: 20px;
    }
    .grid-container .grid-item .community-icon {
      font-size: 30px;
    }
    .grid-container .grid-item .community-text {
      font-weight: bold;
      margin-top: 10px;
    }
    .shape-container {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100px;
      height: 100px;
      background-color: white;
      margin: 5px;
      border: 1px solid black;
    }
    .shape {
      width: 80%;
      height: 80%;
      transition: all 1s ease;
      cursor: pointer;
    }
    .container {
      position: relative;
      width: 150px;
      height: 200px;
      margin: 20px auto;
    }
    .hexagon {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 60px;
      height: 34.64px;
      background-color: #00b3b3;
      transition: all 1s ease;
      cursor: pointer;
      clip-path: polygon(50% 0%, 90.5% 25%, 90.5% 75%, 50% 100%, 9.5% 75%, 9.5% 25%);
    }
    #left-hexagon {
      top: calc(50% - 27px);
      left: calc(50% - 24px);
      background-color: #008c8c;
    }
    #right-hexagon {
      top: calc(50% + 27px);
      left: calc(50% + 24px);
      background-color: #00a6a6;
    }
    .text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 10px;
      font-weight: bold;
      color: white;
    }
    .container:hover .new-page-link {
      display: block;
    }
    .container {
      position: relative;
      width: 150px;
      height: 200px;
      margin: 20px auto;
    }
    .pentagon {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 60px;
      height: 61.51px;
      background-color: #00b3b3;
      transition: all 1s ease;
      cursor: pointer;
      clip-path: polygon(50% 0%, 100% 38.36%, 82.06% 100%, 17.94% 100%, 0% 38.36%);
    }
    #left-pentagon {
      top: calc(50% - 16px);
      left: calc(50% - 81px);
      background-color: #008c8c;
      transform: rotate(-32deg);
    }
    #right-pentagon {
      top: calc(50% + -16px);
      left: calc(50% - -21px);
      background-color: #00a6a6;
      transform: rotate(32deg);
    }
    .text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 10px;
      font-weight: bold;
      color: white;
    }
    .container {
      position: relative;
      width: 150px;
      height: 200px;
      margin: 20px auto;
    }
    .circle {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 45px;
      height: 45px;
      background-color: #00b3b3;
      border-radius: 50%;
      transition: all 1s ease;
      cursor: pointer;
    }
    #center-circle {
      top: calc(50% - 10px);
      left: calc(50% - 12.5px);
      background-color: #00b3b3;
    }
    #left-circle {
      top: calc(50% + 40px);
      left: calc(50% - 40px);
      background-color: #008c8c;
    }
    #triangle {
      position: absolute;
      top: calc(50% + 10px);
      left: calc(50% - 50px);
      width: 0;
      height: 0;
      border-left: 30px solid transparent;
      border-right: 30px solid transparent;
      border-bottom: 70px solid #00a6a6;
      transition: all 1s ease;
      cursor: pointer;
    }
    .container {
      position: relative;
      width: 250px;
      height: 200px;
      margin: 20px auto;
    }
    .rectangle {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #00b3b3;
      transition: all 1s ease;
      cursor: pointer;
    }
    #left-rectangle {
      top: calc(50% - 21px);
      left: calc(50% - 65px);
      background-color: #008c8c;
      width: 50px;
      height: 21px;
    }
    #right-rectangle {
      top: calc(50% - 48px);
      left: calc(50% + -65px);
      background-color: #00a6a6;
      width: 70px;
      height: 14px;
    }
    .triangle {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 0;
      height: 0;
      transition: all 1s ease;
      cursor: pointer;
    }
    #top-triangle {
      top: calc(50% - 75px);
      left: calc(50% - 65px);
      border-bottom: 20px solid #008c8c;
      border-left: 10px solid transparent;
      border-right: 10px solid transparent;
    }
    #bottom-triangle {
      top: calc(50% + -88px);
      left: calc(50% - 65px);
      border-top: 10px solid white;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
    }
    #additional-triangle {
      top: calc(50% + -2px);
      left: calc(50% - 65px);
      border-bottom: 10px solid white;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
    }.container {
      position: relative;
      width: 250px;
      height: 200px;
      margin: 20px auto;
    }
    .rectangle {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #00b3b3;
      transition: all 1s ease;
      cursor: pointer;
    }
    #left-rectangle {
      top: calc(50% - 21px);
      left: calc(50% - 65px);
      background-color: #008c8c;
      width: 50px;
      height: 21px;
      z-index: 3;
    }
    #right-rectangle {
      top: calc(50% - 48px);
      left: calc(50% - 65px);
      background-color: #00b3b3;
      width: 70px;
      height: 14px;
      z-index: 7;
    }
    #duplicated-rectangle {
      top: calc(50% - -14px);
      left: calc(50% + -65px);
      background-color: #008c8c;
      width: 50px;
      height: 21px;
      z-index: 3;
    }
    .triangle {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 0;
      height: 0;
      transition: all 1s ease;
      cursor: pointer;
    }
    #top-triangle {
      top: calc(50% - 75px);
      left: calc(50% - 65px);
      border-top: 9px solid white;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
      z-index: 8;
    }
    #bottom-triangle {
      top: calc(50% - 70px);
      left: calc(50% - 65px);
      border-top: 9px solid #00b3b3;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
      z-index: 8;
    }
    #additional-triangle {
      top: calc(50% - 2px);
      left: calc(50% - 65px);
      border-top: 9px solid white;
      border-left: 5px solid transparent;
      border-right: 5px solid transparent;
      z-index: 8;
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
    }
    footer {
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
    @media (max-width: 768px) {
      header h1 {
        font-size: 30px;
      }
      .hub-card {
        width: 90%;
      }
    }
    @media (max-width: 480px) {
      header h1 {
        font-size: 25px;
      }
      .hub-card {
        width: 100%;
      }
      .grid-container {
        grid-template-columns: repeat(2, 1fr);
      }
    }
  </style><script async src="https://www.googletagmanager.com/gtag/js?id=G-RZG8MP5HRX"></script>
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
    <span class="box"><a href="https://docs.google.com/forms/d/e/1FAIpQLScrHwrJjCwCha1DkU4ZNGvWP2zR41vlqTsyVuK-prMGZjFgQQ/viewform?embedded=true" target="_blank">Here</a></span>
  </div>
  <div class="login">
    <a href="#">Login</a>
    <div class="tooltip">
      You don't need to Sign Up! You are already a Member of Our Community. Save that time browsing what's on offer this week!
    </div>
  </div>
  <h1 class="hub-title">Community Business <br> Hub</h1>
  <div class="social">
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
      </a>
    </div>
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
      </a>
    </div>
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/instagram-new.png" alt="Instagram">
      </a>
    </div>
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/twitter.png" alt="Twitter">
      </a>
    </div>
  </div>
</header><div class="hub-card">
  <h1>Message From The Team</h1>
  <p>Hi There, At The Hub We Have A Team Of Your Local Community Members Who Have Built This Hub For You ! To Help Local Community And Local Business Get Together And Share Eachothers Skills ! </p>
  </div><div class="grid-container">
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/Elderly.assistance/';">
    <i class="community-icon">👵👴🏽</i>
    <p class="community-text">Elderly Assistance</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/Personalized.Exchange.And.Free.Services/';">
    <i class="community-icon">🤝</i>
    <p class="community-text">Community Giveaway</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/The.Community.Graffiti.Wall/';">
    <i class="community-icon">🎨</i>
    <p class="community-text">The Community Graffiti Wall</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/Vintage.High.Street/';">
    <i class="community-icon">📸</i>
    <p class="community-text">Our Vintage Shop Memories</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/Help/';">
    <i class="community-icon">🏠</i>
    <p class="community-text">Help Our Homeless</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/The.Hub/';">
    <i class="community-icon">💼</i>
    <p class="community-text">Encouraging Young Entrepreneurship</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/Personalized.Web.Pages/'">
    <i class="community-icon">🌐</i>
    <p class="community-text">FREE Web Pages, Every Month</p>
  </div>
  <div class="grid-item community-item" onclick="window.location.href = 'https://oavo33.github.io/White.Paper/'">
    <i class="community-icon">📝</i>
    <p class="community-text">White Paper</p>
    <p class="hover-text">Want to Know how Our Community will flourish BY local business? Please read: Section 6.4, That's how our Community gets paid! The more we interact with Local Business, The more we get Paid by Them, Pop in say Thanks</p>
  </div>
</div><div class="grid-wrapper">
  <div class="grid-container">
    <div class="container">
      <div id="left-rectangle" class="rectangle"></div>
      <div id="right-rectangle" class="rectangle"></div>
      <div id="top-triangle" class="triangle"></div>
      <div id="bottom-triangle" class="triangle"></div>
      <div id="additional-triangle" class="triangle"></div></div>
    <div class="container">
      <div id="center-pentagon" class="pentagon">
        <span class="text">Jakes<br>Gardens</span>
      </div>
      <div id="left-pentagon" class="pentagon">
        <span class="text">Rule</span>
      </div>
      <div id="right-pentagon" class="pentagon">
        <span class="text">Now</span>
      </div>
    </div>
    <div class="container">
      <div id="center-hexagon" class="hexagon">
        <span class="text">Jakes<br>Gardens</span>
      </div>
      <div id="left-hexagon" class="hexagon">
        <span class="text">Rule</span>
      </div>
      <div id="right-hexagon" class="hexagon">
        <span class="text">Now</span>
      </div>
    </div><div class="container">
      <div id="center-circle" class="circle"></div>
      <div id="left-circle" class="circle"></div>
      <div id="triangle"></div>
    </div>
  </div>
</div><div class="grid-wrapper">
    <div class="grid-container">
      <div class="container">
        <div id="left-rectangle" class="rectangle"></div>
        <div id="right-rectangle" class="rectangle"></div>
        <div id="duplicated-rectangle" class="rectangle"></div>
        <div id="top-triangle" class="triangle"></div>
        <div id="bottom-triangle" class="triangle"></div>
        <div id="additional-triangle" class="triangle"></div>
      </div>
    </div>
  </div><footer>
  <div class="footer-container">
    <div class="box" onclick="window.location.href = 'https://oavo33.github.io/GitHubz/';">
      <h3>What Do You Think About Our Community Hub?</h3>
    </div>
    <div class="box" onclick="scrollToTop()">🚀</div>
  </div>
  <div class="footer-container">
    <p>&copy; 2023 Lofties. All rights reserved.</p>
  </div>
</footer><script>
leftRectangle.addEventListener("click", moveRectangleAndTriangles);
rightRectangle.addEventListener("click", moveRectangleAndTriangles);
topTriangle.addEventListener("click", moveRectangleAndTriangles);
bottomTriangle.addEventListener("click", moveRectangleAndTriangles);
additionalTriangle.addEventListener("click", moveRectangleAndTriangles);
var centerCircle = document.getElementById("center-circle");
var leftCircle = document.getElementById("left-circle");
var triangle = document.getElementById("triangle");
function moveCircleAndTriangle() {
  centerCircle.style.transform = "translate(-50%, -50%) translateX(1px) translateY(5px)";
  leftCircle.style.transform = "translate(-50%, -50%) translateX(12px) translateY(-45px)";
  triangle.style.transform = "translate(-50%, -50%) translateX(30px) translateY(25px) rotate(180deg)";
  setTimeout(function() {
    // window.location.href = "https://example.com";
  }, 1000); 
}
centerCircle.addEventListener("click", moveCircleAndTriangle);
leftCircle.addEventListener("click", moveCircleAndTriangle);
triangle.addEventListener("click", moveCircleAndTriangle);
var centerPentagon = document.getElementById("center-pentagon");
var leftPentagon = document.getElementById("left-pentagon");
var rightPentagon = document.getElementById("right-pentagon");
function movePentagons() {
  centerPentagon.style.transform = "translate(-50%, -50%) translateY(0px)";
  leftPentagon.style.transform = "translate(-50%, -50%) translateX(54px) translateY(-25px) rotate(36deg)";
  rightPentagon.style.transform = "translate(-50%, -50%) translateX(-22px) translateY(68px) rotate(-38deg)";setTimeout(function() {
    // window.location.href = "https://example.com";
  }, 1000);
}
centerPentagon.addEventListener("click", movePentagons);
leftPentagon.addEventListener("click", movePentagons);
rightPentagon.addEventListener("click", movePentagons);
var centerHexagon = document.getElementById("center-hexagon");
var leftHexagon = document.getElementById("left-hexagon");
var rightHexagon = document.getElementById("right-hexagon");
function moveHexagons() {
  centerHexagon.style.transform = "translate(-50%, -50%) translateY(0px)";
  leftHexagon.style.transform = "translate(-50%, -50%) translateX(48px) translateY(54px) rotate(-360deg)";
  rightHexagon.style.transform = "translate(-50%, -50%) translateX(-48px) translateY(-54px) rotate(360deg)";
  setTimeout(function() {
    // window.location.href = "https://example.com";
  }, 1000);
}
centerHexagon.addEventListener("click", moveHexagons);
leftHexagon.addEventListener("click", moveHexagons);
rightHexagon.addEventListener("click", moveHexagons);
</script>
</body>
</html>
