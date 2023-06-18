<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Hub</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');
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
      padding: 50px 20px;
      text-align: center;
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    header .hub-title {
      font-size: 38px;
      color: white;
      font-weight: bold;
    }
    header div.hub-card-title {
      font-size: 38px;
      color: white;
      margin: 0;
      margin-top: 20px;
      font-weight: bold;
    }
    .header .social {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: center;
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  background: none;
  margin-top: 20px;
}
.header .social div:not(:last-child) {
  margin-right: 20px;
}
.header .social div a {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-decoration: none;
  background: none;
  position: relative;
}
.header .social div a span {
  display: none;
  position: absolute;
  top: -35px;
  left: 50%;
  transform: translateX(-50%);
  margin-top: 5px;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  font-weight: bold;
  color: #00b3b3;
  white-space: nowrap;
}
.header .social div a:hover span {
  display: block;
}
    .login {
      position: absolute;
      top: 14px;
      right: 14px;
      display: flex;
      align-items: center;
    }
    .login button {
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      padding: 5px 10px;
      border-radius: 30px;
      font-family: 'Roboto', sans-serif;
      font-size: 14px;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
      cursor: pointer;
      outline: none;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      transition: background-color 0.3s ease-in-out, transform 0.2s ease-in-out;
    }
    .login button:hover {
      background-color: #008080;
      transform: scale(1.14);
    }
    .login button:active {
      transform: scale(0.95);
    }
    .tooltip {
      position: absolute;
      top: 100%;
      right: 99%;
      transform: translateX(50%);
      width: 200px;
      background-color: #f2f2f2;
      border: 1px solid #00b3b3;
      border-radius: 5px;
      padding: 10px;
      font-size: 14px;
      color: #333333;
      text-align: center;
      visibility: hidden;
      opacity: 0;
      transition: visibility 0s, opacity 0.3s ease-in-out;
      z-index: 10;
      font-family: 'Roboto', sans-serif;
    }
    .login:hover .tooltip {
      visibility: visible;
      opacity: 1;
    }
    .hub-card {
      background: linear-gradient(to bottom, #008080, #00b3b3);
      border-radius: 10px;
      border: 2px solid #ffffff;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      padding: 10px;
      text-align: center;
      max-width: 280px;
      width: 65%;
      margin: 0 auto;
      margin-top: -55px;
      position: relative;
      z-index: 2;
    }
    .hub-card .hub-card-title {
      font-size: 16px;
      margin-top: 0;
      font-weight: bold;
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
      font-size: 11px;
      transform: rotate(-7deg);
      top: 2%;
      color: white;
    }
    .grid-item .-text {
      font-size: 18px;
      margin: 0;
      color: #333333;
      cursor: pointer;
      transition: color 0.3s ease-in-out;
    }
    .grid-item .-text:hover {
      color: #00b3b3;
      text-decoration: underline;
    }
    .grid-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 2fr));
      grid-gap: 20px;
      padding: 20px;
      max-width: 1000px;
      margin: 0 auto;
    }
    .grid-item {
      background-color: #ffffff;
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      cursor: pointer;
      position: relative;
    }
    .grid-item h3 {
      font-size: 16px;
      margin-top: 0;
      margin-bottom: 10px;
      color: #00b3b3;
    }
    .grid-item p {
      font-size: 14px;
      margin-bottom: 10px;
      color: #333333;
    }
    .grid-item .community-text {
      font-size: 14px;
      color: #00b3b3;
      font-weight: bold;
    }
    /* Footer Styles */
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
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
      padding: 20px;
      text-align: center;
      margin: 10px;
      cursor: pointer;
    }
    .footer-container .box h3 {
      font-size: 18px;
      margin: 0;
      color: #ffffff;
    }
    .footer-container .box p {
      font-size: 14px;
      margin: 10px 0 0;
      color: #ffffff;
    }
    .footer-container .box:first-child {
      border: 1px solid #ffffff;
    }
    .footer-container .box:last-child {
      border: 1px solid #ffffff;
    }
    .tcbhg {
      text-align: center;
      margin-top: 20px;
    }
    .tcbhg a {
      color: #00b3b3;
      text-decoration: none;
    }
    .tcbhg a:hover {
      text-decoration: underline;
    }
    .graffiti-button {
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      padding: 2px 4px;
      border-radius: 30px;
      font-family: 'Roboto', sans-serif;
      font-size: 10px;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
      cursor: pointer;
      outline: none;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      transition: background-color 0.3s ease-in-out, transform 0.2s ease-in-out;
    }
    .graffiti-button:hover {
      background-color: #008080;
      transform: scale(1.05);
    }
    .graffiti-button:active {
      transform: scale(0.95);
    }
    .new-heading {
      font-size: 18px;
      color: #00b3b3;
      margin-top: 0;
    }
    .new-heading+p {
      font-size: 10px;
      margin-bottom: 10px;
      color: #00b3b3;
    }
    .cta-button {
      display: inline-block;
      background-color: #00b3b3;
      color: #ffffff;
      border: none;
      padding: 2px 4px;
      border-radius: 14px;
      font-family: 'Roboto', sans-serif;
      font-size: 10px;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
      cursor: pointer;
      outline: none;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      transition: background-color 0.3s ease-in-out, transform 0.2s ease-in-out;
      margin-top: 5px;
    }
    .cta-button:hover {
      background-color: #008080;
      transform: scale(1.05);
    }
    .cta-button:active {
      transform: scale(0.95);
    }
    /* Social Media Icons */
    .social-icons {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 20px;
    }
    .social-icons a {
      display: inline-block;
      margin: 0 5px;
      width: 30px;
      height: 30px;
      border-radius: 50%;
      background-color: #00b3b3;
      text-decoration: none;
      color: #ffffff;
      font-size: 20px;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: background-color 0.3s ease-in-out, transform 0.2s ease-in-out;
    }
    .social-icons a:hover {
      background-color: #008080;
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
  <div class="login">
  <button class="custom-class">Login</button>
  <div class="tooltip">
    You don't need to Sign Up! You are already a Member of Our Community. Save that time browsing what's on offer this week!
  </div>
</div>
  <h1 class="hub-title">The Community Business Hub</h1>
  <div class="graffiti">
    This is your Hub !<br>
    Do you want to change It ?<br>
    Submit Request <br>
    <span class="box"><button class="graffiti-button" onclick="window.open('https://docs.google.com/forms/d/e/1FAIpQLScrHwrJjCwCha1DkU4ZNGvWP2zR41vlqTsyVuK-prMGZjFgQQ/viewform?embedded=true')">Here</button></span>
  </div>
  <div class="social">
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
        <span>YouTube</span>
      </a>
    </div>
    <div>
      <a href="#">
        <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
        <span>Facebook</span>
      </a>
    </div>
  </div>
</header>
<div class="hub-card">
  <div class="hub-card-title">Message From The Team</div>
  <p>Hi there! At The Hub, we have a team of your local community members who have built this hub for you! We aim to help the local community and local businesses come together and share each other's skills.</p>
</div>
<div class="grid-container">
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_1')">
    <a class="community-item" href="https://oavo33.github.io/Elderly.assistance/"><p class="community-text">Elderly Assistance</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_2')">
    <a class="community-item" href="https://oavo33.github.io/Personalized.Exchange.And.Free.Services/"><p class="community-text">Community Giveaway</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_3')">
    <a class="community-item" href="https://oavo33.github.io/The.Community.Graffiti.Wall"><p class="community-text">The Community Graffiti Wall</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_4')">
    <a class="community-item" href="https://oavo33.github.io/Vintage.High.Street/"><p class="community-text">Our Vintage Shop Memories</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_5')">
    <a class="community-item" href="https://oavo33.github.io/Help/"><p class="community-text">Help Our Homeless</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_6')">
    <a class="community-item" href="https://oavo33.github.io/The.Hub/"><p class="community-text">Encouraging Young Business</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_7')">
    <a class="community-item" href="https://oavo33.github.io/Personalized.Web.Pages/"><p class="community-text">FREE Web Pages, Every Month</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)" style="background-image: url('IMAGE_URL_8')">
    <a class="community-item" href="https://oavo33.github.io/White.Paper/"><p class="community-text">White Paper</p>
    </a>
  </div>
  <div class="grid-item" onclick="changeColor(this)">
  <div class="new-heading">Let's Go!</div>
  <p>Hey community! As your cheeky window cleaner, I've been auditing local businesses and here's what I found. The more we Subscribe, Like, and Follow Our Hub, the more we help them thrive. When we support them, they can support us in return. So let's subscribe, like, follow, and spread the word about their fantastic services. Together, we can ensure the success of our local businesses. Stay cheeky and support local! - The Cheeky Window Cleaner</p>
  <a href="https://www.facebook.com/myprofile" class="cta-button">Add Us On Facebook</a>
  <a href="https://www.youtube.com/mychannel" class="cta-button">Subscribe On YouTube</a>
</div><div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 140% ; background-repeat: no-repeat; background-position: center;" >
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div><div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div><div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div><div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
  <div class="grid-item" style="background-image: url('https://i.imgur.com/gT1Sbd4.png'); background-size: 100% ; background-repeat: no-repeat; background-position: center;" onclick="changeColor(this)">
    <p class="-text" onclick="window.location.href='1'">New Button 1</p>
    <p class="-text" onclick="window.location.href='URL_HERE'">New Button 6</p>
  </div>
</div>
<footer>
    <div class="footer-container">
      <div class="box">
        <h3>Contact</h3>
        <p>Email: contact@thehub.com</p></div>
      <div class="box">
  <h3>Terms and conditions</h3>
  <p>By using The Hub, you agree to our <a href="https://example.com/terms" style="color: pink;">Terms of Service</a> and Privacy Policy. Please read them carefully before accessing or using our platform.</p>
</div><div class="box" onclick="window.location.href = 'https://oavo33.github.io/GitHubz/';">
        <h3>What Do You Think About Our Community Hub?</h3>
      </div><div class="box">
        <h3>Follow Us</h3>
        <div class="social">
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/youtube.png" alt="YouTube">
          </a>
          <a href="#">
            <img src="https://img.icons8.com/office/30/FF0000/facebook-new.png" alt="Facebook">
          </a>
        </div>
      </div>
      <div class="box back-to-top" onclick="scrollToTop()">To The Top</div><p>&copy; 2023 Lofties. All rights reserved.</p>
    </div>
    <div class="tcbhg">
  <p>
    <a href="https://example.com/privacy-policy" style="color: pink;">Privacy Policy</a>
  </p>
  <p>
    <a href="https://example.com/guide-to-copywriting" style="color: pink;">The Community Business Hub's Guide To Copywriting</a>
  </p>
</div>
  </footer>
<script>
  function scrollToTop() {
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  function changeColor(element) {
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
  buttons.forEach(function (button) {
    button.addEventListener('click', stopPropagation);
  });
  var gridItems = document.querySelectorAll('.grid-item');
  gridItems.forEach(function (gridItem) {
    var itemButtons = gridItem.querySelectorAll('.community-text');
    itemButtons.forEach(function (itemButton) {
      itemButton.addEventListener('click', stopPropagation);
    });
  });
</script>
</body>
</html>