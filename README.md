<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Community Graffiti Wall</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f2f2f2;
    }
    header {
      background-color: #ff6699;
      color: #ffffff;
      padding: 20px;
      text-align: center;
      border-bottom: 2px solid #ffffff;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.4);
      transform-style: preserve-3d; 
      perspective: 500px; 
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }
    h1 {
      font-size: 32px;
      color: #ffcc00;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 2px;
      transform: translateZ(40px);
      animation: rotateHeader 10s infinite linear; 
    }
    @keyframes rotateHeader {
      0% { transform: translateZ(40px) rotateY(0); }
      100% { transform: translateZ(40px) rotateY(1turn); }
    }
    .brick-wall {
      background-color: #ff6699;
      padding: 20px;text-align: center;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .container {
      max-width: 960px;
      width: 100%;
      margin: 0 auto;
      padding: 20px;
      box-sizing: border-box;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }
    .bricks-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      background-color: #ff6699;
      padding: 20px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .brick {
      background-color: #8B0000;
      width: 20px;
      height: 10px;
      display: inline-block;
      margin: 1px;
    }
    h1 {
      font-size: 32px;
      color: #ffcc00;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 2px;
    }
    p {
      font-size: 16px;
      margin-bottom: 20px;
      color: #333333;
    }
    .appealing-paragraph {
      font-size: 20px;
      line-height: 1.5;text-align: center;
      color: #333333;
      margin: 40px 0;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .highlight {
      color: #ff6699;
      font-weight: bold;
    }
    .graffiti-wall {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 40px;
    }
    .graffiti-item {
      color: #ffffff;
      border-radius: 5px;
      padding: 10px 20px;
      margin: 10px;
      font-size: 14px;
      font-weight: bold;
      text-transform: uppercase;
      font-family: Arial, sans-serif;
      letter-spacing: 1px;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.4);
      cursor: pointer;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
      animation: borderAnimation 2s infinite;
    }
    @keyframes borderAnimation {
      0% { border: 2px solid #ffcc00; }
      50% { border: 2px solid #ff6699; }
      100% { border: 2px solid #ffcc00; }
    }
    .form-container {
      max-width: 400px;
      margin: 0 auto;
      margin-bottom: 40px;
    }
    input[type="text"] {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      font-size: 14px;
    }
    .gallery-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .gallery-item {
      flex-basis: 150px;
      height: 150px;
      background-color: #ffcc00;
      margin: 10px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    footer {
      padding: 80px 0;
      background-color: #ff6699;
      color: #ffffff;
      text-align: center;
      clip-path: polygon(50% 15%, 90% 20%, 100% 50%, 90% 80%, 50% 100%, 10% 80%, 0% 50%, 10% 20%);
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }
    footer p {
      margin: 0;
    }
    .footer-wrapper {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      gap: 2px;
      margin-bottom: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .footer-section {
      border: 1px solid maroon;
      padding: 2px;
      border-radius: 10px;
      flex: 1 1 300px;
      max-width: 300px;
      text-align: center;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
    }
    .footer-title {
      font-size: 12px;
      margin-bottom: 10px;
      color: maroon;
      text-transform: uppercase;
    }
    .footer-text {
      font-size: 12px;
    }
    .footer-social {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 2px;
    }
    .footer-social img {
      margin: 0 5px;
      width: 20px;
      height: 20px;
    }
    .footer-container {
      text-align: center;
    }
    .tcbhg {
      text-align: center;
      margin-top: 20px;
    }
    .tcbhg a {
      color: #8b0000;
      text-decoration: none;
    }
    .tcbhg a:hover {
      text-decoration: underline;
    }
  </style>
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-RZG8MP5HRX"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag() { dataLayer.push(arguments); }
    gtag('js', new Date());
    gtag('config', 'G-RZG8MP5HRX');
  </script>
</head>
<body>
  <header class="brick-wall">
    <div class="container">
      <div class="social">
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
        </a>
        <a href="#">
          <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
        </a>
      </div>
      <div class="bricks-container"></div>
      <h1>The Graffiti Collective</h1>
    </div>
  </header>
  <p class="appealing-paragraph">
    Welcome to our vibrant and interactive <strong class="highlight">"Graffiti Wall"</strong> feature! It's all about you, our incredible community members. Unleash your creativity and leave your mark on our digital canvas. Submit your unique nickname, and watch with pride as it becomes a timeless part of our thriving hub. This innovative idea was born from our deep commitment to fostering engagement and inclusivity among individuals of all ages. Join us in creating an unforgettable tapestry of identities that will forever be associated with our remarkable community.
  </p>
  <div class="graffiti-wall" id="graffiti-wall">
  </div>
  <div class="form-container">
    <h2>Submit Your Nickname</h2>
    <input type="text" id="nickname-input" placeholder="Enter your nickname">
    <button onclick="submitNickname()">Submit</button>
  </div>
  <h3>Imagine Our Wall On Your House! #MaybeOneDay</h3>
  <div class="gallery-container">
    <div class="gallery-item"></div>
    <div class="gallery-item"></div>
    <div class="gallery-item"></div>
    <div class="gallery-item"></div>
  </div>
  <footer>
    <div class="footer-wrapper">
      <div class="footer-section">
        <h3 class="footer-title">Connect</h3>
        <p class="footer-text">Email: connect@thehub.com</p><div class="footer-social">
          <a href="#">
            <img src="https://img.icons8.com/office/30/0000FF/youtube.png" alt="YouTube">
          </a>
          <a href="#">
            <img src="https://img.icons8.com/office/30/0000FF/facebook-new.png" alt="Facebook">
          </a>
        </div>
      </div><div class="footer-section">
        <h3 class="footer-title">Know More About Us</h3>
        <p class="footer-text">Terms of Service and Privacy Policy. Please read them thoroughly before accessing or using our platform.</p>
      </div>
      <div class="footer-section">
        <div class="footer-container">
          <p>&copy; 2023 Lofties. All rights reserved.</p>
        </div>
      </div>
      <div class="footer-section">
        <div class="tcbhg">
          <p>
            <a href="https://example.com/guide-to-copywriting">The Community Business Hub's Guide To Copywriting</a>
          </p>
        </div>
      </div>
    </div>
  </footer>
  <script>
    function getRandomRainbowColor() {
      var colors = [
        "#FF0000", // Red
        "#FF7F00", // Orange
        "#FFFF00", // Yellow
        "#00FF00", // Green
        "#0000FF", // Blue
        "#4B0082", // Indigo
        "#8B00FF" // Violet
      ];
      return colors[Math.floor(Math.random() * colors.length)];
    }
    function addGraffitiItem() {
      var graffitiWall = document.getElementById('graffiti-wall');
      var graffitiItem = document.createElement('div');
      graffitiItem.className = 'graffiti-item';
      graffitiItem.style.backgroundColor = getRandomRainbowColor();
      graffitiItem.innerText = 'Nickname ' + (graffitiWall.childElementCount + 1);
      graffitiWall.appendChild(graffitiItem);
    }
    for (var i = 0; i < 25; i++) {
      addGraffitiItem();
    }
    var graffitiItems = document.getElementsByClassName('graffiti-item');
    for (var i = 0; i < graffitiItems.length; i++) {
      graffitiItems[i].addEventListener('click', function() {
        this.style.backgroundColor = getRandomRainbowColor();
      });
    }
    function submitNickname() {
      var nicknameInput = document.getElementById('nickname-input');
      var nickname = nicknameInput.value.trim();
      if (nickname !== '') {
        var graffitiWall = document.getElementById('graffiti-wall');
        var graffitiItem = document.createElement('div');
        graffitiItem.className = 'graffiti-item';
        graffitiItem.style.backgroundColor = getRandomRainbowColor();
        graffitiItem.innerText = nickname;
        graffitiWall.appendChild(graffitiItem);
        nicknameInput.value = '';
      }
    }
    function generateBricks() {
      var bricksContainer = document.querySelector('.bricks-container');
      var numBricks = 114;
      for (var i = 0; i < numBricks; i++) {
        var brick = document.createElement('div');
        brick.className = 'brick';
        bricksContainer.appendChild(brick);
      }
    }
    generateBricks();
  </script>
</body>
</html>
