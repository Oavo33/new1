<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Hub</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');body {
      font-family: 'Roboto', sans-serif;
      font-size: 14px;
      background-color: #f2f2f2;
      color: #333333;
      margin: 0;
      padding: 0;
    }header {
      background: linear-gradient(to bottom, #00b3b3, #008080);
      padding: 40px 20px;
      text-align: center;
      position: relative;
    }header .hub-title {
      font-size: 38px;
    }header h1 {
      font-size: 38px;
      color: #ffffff;
      margin: 0;
    }.social {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
    }.social div {
      margin-bottom: 5px;
    }.social div a {
      display: flex;
      align-items: center;
      text-decoration: none;
    }.social div a img {
      width: 30px;
      height: 30px;
    }.login {
      position: absolute;
      top: 14px;
      right: 14px;
      display: flex;
      align-items: center;
      font-weight: bold;
      text-decoration: none;
      color: red;
    }.login a {
      color: yellow !important;
    }.login:hover .tooltip {
      visibility: visible;
      opacity: 1;
    }.tooltip {
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
    }.hub-card {
      background: linear-gradient(to bottom, #008080, #00b3b3);
      border-radius: 10px;
      border: 2px solid #ffffff;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      padding: 10px;
      text-align: center;
      max-width: 341.4px;
      width: 65%;
      margin: 0 auto;
      margin-top: -136px;
      position: relative;
      z-index: 2;
    }.hub-card h1 {
      font-size: 16px;
      margin-top: 0;
      margin-bottom: 2px;
      color: #ffffff;
    }.hub-card p {
      font-size: 14px;
      margin-bottom: 2px;
      color: #ffffff;
    }.graffiti {
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
    }.grid-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      grid-gap: 10px;
      max-width: 800px;
      margin: 10px auto;
      padding: 0 10px;
    }.grid-item {
      border-radius: 10px;
      padding: 10px;
      text-align: center;
      border: 1px solid #00b3b3;
    }.community-item {
      padding: 10px;
      display: inline-flex;
      flex-direction: column;
      align-items: center;
      text-decoration: none;
      color: #333333;
    }.community-icon {
      font-size: 30px;
      margin-bottom: 10px;
    }.community-text {
      font-size: 14px;
      font-weight: 500;
      margin: 0;
      color: #00b3b3;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
    }footer {
      background: linear-gradient(to bottom, #ffffff, #00b3b3);
      padding: 35px;
      color: #ffffff;
      text-align: center;
      font-size: 14px;
    }.footer-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
    }.footer-container .box {
      background-color: #00b3b3;
      color: #ffffff;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2), 0 6px 6px rgba(0, 0, 0, 0.2);
      padding: 10px;
      text-align: center;
      margin: 10px;
      cursor: pointer;
    }.footer-container .box h3 {
      margin: 0;
    }.footer-container .box:first-child {
      border: 1px solid #ffffff;
    }.footer-container .box:last-child {
      border: 1px solid #ffffff;
    }@media only screen and (max-width: 600px) {
      header .hub-title {
        font-size: 24px;
      }header h1 {
        font-size: 24px;
      }.hub-card {
        width: 100%;
        margin-top: 0;
      }.grid-item {
        width: 100%;
      }.community-icon {
        font-size: 24px;
      }.community-text {
        font-size: 12px;
      }.footer-container .box {
        width: 100%;
      }
    }@media only screen and (min-width: 601px) and (max-width: 1024px) {
      header .hub-title {
        font-size: 32px;
      }header h1 {
        font-size: 32px;
      }.hub-card {
        width: 75%;
        margin-top: -100px;
      }.grid-item {
        width: calc((100% - 30px) / 2);
      }.community-icon {
        font-size: 28px;
      }.community-text {
        font-size: 14px;
      }.footer-container .box {
        width: calc((100% - 30px) / 2);
      }
    }@media only screen and (min-width: 1025px) {
      header .hub-title {
        font-size: 38px;
      }header h1 {
        font-size: 38px;
      }.hub-card {
        width: 65%;
        margin-top: -136px;
      }.grid-item {
        width: calc((100% - 40px) / 3);
      }.community-icon {
        font-size: 30px;
      }.community-text {
        font-size: 16px;
      }.footer-container .box {
        width: calc((100% - 40px) / 3);
      }
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
  <div class="hub-title">The Community <br> Business Hub</div>
  <div class="social">
    <a href="#"><img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube"></a>
    <a href="#"><img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook"></a></div>
</header><div class="hub-card">
  <h1>Message From The Team</h1>
  <p>Hi there! At The Hub, we have a team of your local community members who have built this hub for you! We aim to help the local community and local businesses come together and share each other's skills.</p>
</div><div class="grid-container">
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/Elderly.assistance/">
      <i class="community-icon">👵👴🏽</i>
      <p class="community-text">Elderly Assistance</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/Personalized.Exchange.And.Free.Services/">
      <i class="community-icon">🤝</i>
      <p class="community-text">Community Giveaway</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/The.Community.Graffiti.Wall">
      <i class="community-icon">🎨</i>
      <p class="community-text">The Community Graffiti Wall</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/Vintage.High.Street/">
      <i class="community-icon">📸</i>
      <p class="community-text">Our Vintage Shop Memories</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/Help/">
      <i class="community-icon">🏠</i>
      <p class="community-text">Help Our Homeless</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/The.Hub/">
      <i class="community-icon">💼</i>
      <p class="community-text">Encouraging Young Business</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item" href="https://oavo33.github.io/Personalized.Web.Pages/">
      <i class="community-icon">🌐</i>
      <p class="community-text">FREE Web Pages, Every Month</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
  <a class="community-item" href="https://oavo33.github.io/White.Paper/">
    <i class="community-icon">📝</i>
    <p class="community-text" onclick="event.stopPropagation();">White Paper</p>
  </a>
</div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-repeat: no-repeat; background-position: center; background-size: cover; position: relative;">
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>
<div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-repeat: no-repeat; background-position: center; background-size: cover; position: relative;">
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>
<div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-repeat: no-repeat; background-position: center; background-size: cover; position: relative;">
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>
<div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-repeat: no-repeat; background-position: center; background-size: cover; position: relative;">
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>
<div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-repeat: no-repeat; background-position: center; background-size: cover; position: relative;">
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>
  <a class="community-item" style="position: absolute; bottom: -14px; left: 13.14%;">
    <p class="community-text" onclick="window.location.href='1'" style="cursor: pointer;">custom Review</p>
    <p class="community-text" onclick="window.location.href='URL_HERE'" style="cursor: pointer;">Page Review</p>
  </a>
</div>

  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">📚</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">⚽</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎨</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎧</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🌈</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
<div class="grid-item" onclick="changeColor(this)">
    <div class="community-item">
      <i class="community-icon">🌟</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </div>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎯</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎮</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🌺</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🍕</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">📚</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">⚽</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎨</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🎧</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
    <a class="community-item">
      <i class="community-icon">🌈</i>
      <p class="community-text" onclick="window.location.href='1'">New Button 1</p>
      <p class="community-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
    </a>
  </div>
</div><footer>
  <div class="footer-container">
    <div class="box">
      <h3>Contact</h3>
      <p>Email: contact@thehub.com</p>
      <p>Phone: 123-456-7890</p>
    </div>
    <div class="box">
      <h3>About Us</h3><p>By using The Hub, you agree to our Terms of Service and Privacy Policy. Please read them carefully before accessing or using our platform.</p>
    </div>
  </div><div class="footer-container">
    <div class="box" onclick="window.location.href = 'https://oavo33.github.io/GitHubz/';">
      <h3>What Do You Think About Our Community Hub?</h3>
    </div>
    <div class="box" onclick="scrollToTop()">Back To Top</div>
  </div>
  <div class="footer-container">
    <p>&copy; 2023 Lofties. All rights reserved.</p>
  </div><div class="tcbhg">
  <p>
    <a href="https://example.com/guide-to-copywriting">The Community Business Hub's Guide To Copywriting</a>
  </p>
</div>
</footer>

<script>
  function scrollToTop() {
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }

  function changeColor(element) {
  // Check if the clicked element is the first border box
  if (element.classList.contains('grid-item')) {
    var colors = ['#FF0000', '#FF7F00', '#FFFF00', '#00FF00', '#0000FF', '#8B00FF'];
    var randomColor = colors[Math.floor(Math.random() * colors.length)];
    element.style.backgroundColor = randomColor;
  }
}
  function stopPropagation(event) {
    event.stopPropagation();
  }

  var buttons = document.querySelectorAll('.community-item a');
  buttons.forEach(function(button) {
    button.addEventListener('click', stopPropagation);
  });

  var gridItems = document.querySelectorAll('.grid-item');
  gridItems.forEach(function(gridItem) {
    var itemButtons = gridItem.querySelectorAll('.community-text');
    itemButtons.forEach(function(itemButton) {
      itemButton.addEventListener('click', stopPropagation);
    });
  });
</script>
</body>
</html>
