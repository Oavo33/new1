<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Youth Entrepreneurship Hub</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f2f2f2;
      overflow-x: hidden; 
    }
    .header {
      background: linear-gradient(to bottom, #00b3b3, #008080);
      padding: 20px;
      text-align: center;
      color: #ffffff;
    }
    .logo {
      font-size: 32px;
      font-weight: bold;
      margin: 0;
    }
    .description {
      font-size: 18px;
      margin-top: 10px;
      margin-bottom: 20px;
    }
    .main-content {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;text-align: center;
    }.highlight-box {
      background-color: #ffffff;
      color: #333333;
      border-radius: 10px;
      padding: 40px;
      margin-bottom: 40px;
      box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
    }
    .highlight-title {
      font-size: 32px;
      margin-top: 0;
      margin-bottom: 20px;}.highlight-text {
      font-size: 18px;
      line-height: 1.6;
      margin-bottom: 20px;
    }.cta-button {
      display: inline-block;
      padding: 16px 36px;
      background-color: #00b3b3;
      color: #ffffff;
      font-size: 20px;
      font-weight: bold;
      text-decoration: none;
      border-radius: 50px;
      transition: background-color 0.3s;
      box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.2);
    }
    .cta-button:hover {
      background-color: #008080;
    }
    .secondary-button {
      display: inline-block;
      padding: 4px 9px;
      background-color: #00b3b3;
      color: #ffffff;
      font-size: 14px;
      font-weight: bold;
      text-decoration: none;
      border-radius: 50px;
      transition: background-color 0.3s;
      box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.2);
    }
    .secondary-button:hover {
      background-color: #008080;
    }
    .social {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }
    .social a {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 50px;
      height: 50px;
      margin: 0 8px;
      border-radius: 50%;
      background-color: #00b3b3;
      color: #ffffff;
      text-decoration: none;
      transition: background-color 0.3s;
    }
    .social a:hover {
      background-color: #008080;
    }
    footer {
  background: linear-gradient(to bottom, #00b3b3, #008080);
  padding: 20px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
}
.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}
.footer-container .box {
  background-color: #00b3b3;
  color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  padding: 2px;
  text-align: center;
  margin: 2px;
  cursor: pointer;
  flex: 0 0 auto; 
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0);  
}
  </style>
</head>
<body>
  <div class="header">
    <h1 class="logo">Youth Entrepreneurship Hub</h1>
    <p class="description">Inspiring and empowering young entrepreneurs</p>
    <div class="social">
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
      </a>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
      </a>
    </div>
  </div>
  <div class="main-content">
    <div class="highlight-box">
      <h2 class="highlight-title">Encouraging Young Entrepreneurship</h2>
      <p class="highlight-text">Every year, we provide a platform for aspiring young entrepreneurs in the community. We invite three individuals, regardless of age, to submit their business plans. Once their proposals demonstrate a clear direction and compliance with legal requirements, we offer them the opportunity to launch their own business with full autonomy.</p>
      <p class="highlight-text">To support their ventures, we provide a startup capital of £1000. These young entrepreneurs are free to invest in any legal stocks or materials of their choice.</p>
      <p class="highlight-text">We're thrilled to share that a local lad, <a href="jake.html" style="color: #00b3b3;">Jake</a>, aged 16, has already taken the initiative and started a successful gardening business in the vicinity of St. Cathrienes Hospital. We've been informed about his remarkable endeavor, and we're actively assisting him with his future plans. His inspiring story serves as a testament to the potential and determination of young entrepreneurs in our community.</p>
      <p class="highlight-text">We aim to inspire and support the entrepreneurial aspirations of our young community members, encouraging them to save pocket money and pursue their dreams. Take, for example, the story of a 12-year-old kid who wrote to an Australian scooter company and asked if he could sell their scooters in England. The Australian company agreed, and that 12-year-old kid has now made millions by moving stocks from A to B. It's a true story—Google it!</p>
      <p class="highlight-text">Join us today and be a part of the thriving community of young entrepreneurs!</p>
      <a href="newpage.html" class="cta-button">Get Started</a>
      <br>
      <button id="rainbowButton" class="secondary-button" onclick="addRainbowEffect();">Secondary Button</button>
    </div>
  </div>
  <footer>
    <div class="footer-container">
      <div class="box">
        <h3>Contact</h3>
        <p>Email: contact@thehub.com</p>
      </div>
      <div class="box">
        <h3>About Us</h3>
        <p>By using The Hub, you agree to our Terms of Service and Privacy Policy.<br> Please read them carefully before accessing or using our platform.</p>
      </div>
    </div>
    <div class="footer-container">
      <div class="box" onclick="scrollToTop()">Top Of Page</div>
    </div>
    <div class="footer-container">
      <p>&copy; 2023 Lofties. All rights reserved.</p>
    </div>
    <div class="tcbhg">
      <p>
        <a href="https://example.com/guide-to-copywriting">The Community Business Hub's Guide To Copywriting</a>
      </p>
    </div>
  </footer>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/js/all.min.js"></script>
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-RZG8MP5HRX"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-RZG8MP5HRX');
  </script>
  <script>
    function scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
    function addRainbowEffect() {
      var colors = ['#ff0000', '#ff7f00', '#ffff00', '#00ff00', '#0000ff', '#8b00ff'];
      var button = document.getElementById('rainbowButton');
      var currentIndex = 0;
      var interval = setInterval(function() {
        button.style.backgroundColor = colors[currentIndex];
        currentIndex++;
        if (currentIndex === colors.length) {
          currentIndex = 0;
        }
      }, 200);
      setTimeout(function() {
        clearInterval(interval);
        button.style.backgroundColor = '#00b3b3';
      }, 3000);
    }
  </script>
</body>
</html>
