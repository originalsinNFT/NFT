<html>
<title>W3.CSS Template</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body,h1,h2,h3,h4,h5,h6 {font-family: "Lato", sans-serif;}
body, html {
  height: 100%;
  color: #777;
  line-height: 1.8;
}

/* Create a Parallax Effect */
.bgimg-1, .bgimg-2, .bgimg-3 {
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/* First image (Logo. Full height) */
.bgimg-1 {
  background-image: url('./test1.jpg');
  min-height: 100%;
}

/* Second image (Portfolio) */
.bgimg-2 {
  background-image: url("./test1.jpg");
  min-height: 400px;
}

/* Third image (Contact) */
.bgimg-3 {
  background-image: url("./test1.jpg");
  min-height: 400px;
}

.w3-wide {letter-spacing: 10px;}
.w3-hover-opacity {cursor: pointer;}

/* Turn off parallax scrolling for tablets and phones */
@media only screen and (max-device-width: 1600px) {
  .bgimg-1, .bgimg-2, .bgimg-3 {
    background-attachment: scroll;
    min-height: 400px;
  }
}
</style>
<body>

<!-- Navbar (sit on top) -->
<div class="w3-top">
  <div class="w3-bar" id="myNavbar">
    <a class="w3-bar-item w3-button w3-hover-black w3-hide-medium w3-hide-large w3-right" href="javascript:void(0);" onclick="toggleFunction()" title="Toggle Navigation Menu">
      <i class="fa fa-bars"></i>
    </a>
    <a href="#home" class="w3-bar-item w3-button">HOME</a>
    <a href="#about" class="w3-bar-item w3-button w3-hide-small">About</i></a>
    <a href="https://t.me/noefforttoken" class="w3-bar-item w3-button w3-hide-small">Telegram</i> </a>
    <a href="https://uniswap.info/home" class="w3-bar-item w3-button w3-hide-small">Uniswap</i> </a>
    <a href="#" class="w3-bar-item w3-button w3-hide-small w3-right w3-hover-red">
    </a>
  </div>


<!-- First Parallax Image with Logo Text -->
<div class="bgimg-1 w3-display-container w3-opacity-min" id="home">
  <div class="w3-display-middle" style="white-space:nowrap;">
    <span class="w3-center w3-padding-large w3-black w3-xlarge w3-wide w3-animate-opacity">NO <span class="w3-hide-small">EFFORT</span> TOEKN (EFT)</span>
  </div>
</div>


<!-- Container (About Section) -->
<div class="w3-content w3-container w3-padding-64" id="about">
  <h3 class="w3-center">What is No Effort Token?</h3>
  <p class="w3-center">NFT is... I don't even want to explain since it requires effort 😑. But here is a poem you can read.</p>
    <p class="w3-center">Heart is draining</p>
    <p class="w3-center">Feeling lost and cold</p>
    <p class="w3-center">Where did my ETH go?</p>
    <p class="w3-center">The ETH we had is now dull, forgotten</p>
    <p class="w3-center">Do you even belive in moon or of my token?</p>
    <p class="w3-center">Is something between us or lost the fomo?</p>
    <p class="w3-center">For I still will moon</p>
    <p class="w3-center">but a pajeet can only take so much</p>
    <p class="w3-center">Moon shots cannot live on a one way street</p>
    <p class="w3-center">The more I try to save it</p>
    <p class="w3-center">The less I see effort come from you</p>
    <p class="w3-center">It leaves me with all the weight and an empty heart.</p>
    <p class="w3-center">It leaves me with all the weight and an empty heart.</p>
    <!-- Hide this text on small devices -->
    <div class="w3-col m6 w3-hide-small w3-padding-large">
    </div>
  </div>
</div>



<!-- https://uniswap.info -->
<div class="w3-content w3-container w3-padding-64" id="contact">
  <h3 class="w3-center">How to buy?</h3>
  <div class="w3-row w3-padding-32 w3-section">
    <div class="w3-col m4 w3-container">
      <img src="./log.png" class="w3-image w3-round" style="width:100%">
    </div>
    <div class="w3-col m8 w3-panel">
      <div class="w3-large w3-margin-bottom">
      </div>
      <p>You can buy the EFT on Uniswap using the button</p>
      <form action="/action_page.php" target="_blank">
        <div class="w3-row-padding" style="margin:0 -16px 8px -16px">
         <button onclick="location.href='https://uniswap.info' "class="w3-button w3-black w3-left w3-section" type="button">
            <i class="fa fa-paper-plane" ></i> Uniswap Buy
        </button>
      </form>
    </div>
  </div>
</div>



<h3 class="w3-center">Token Info</h3>
<div>
    <script type="text/javascript" src="https://canvasjs.com/assets/script/canvasjs.min.js"></script>
<div id="chartContainer" style="height: 500px; width: 100%;"></div>




<!-- Footer -->
<footer class="w3-center w3-black w3-padding-64 w3-opacity w3-hover-opacity-off">
  <a href="#home" class="w3-button w3-light-grey"><i class="fa fa-arrow-up w3-margin-right"></i>To the top</a>
  <div class="w3-xlarge w3-section">
    <p>Disclaimer: This is not a financial product that guaranteed profit. The sole purpose of the NFT token is created for FUN!.</p>
  </div>
</footer>
 
<script>
// Modal Image Gallery
function onClick(element) {
  document.getElementById("img01").src = element.src;
  document.getElementById("modal01").style.display = "block";
  var captionText = document.getElementById("caption");
  captionText.innerHTML = element.alt;
}

// Change style of navbar on scroll
window.onscroll = function() {myFunction()};
function myFunction() {
    var navbar = document.getElementById("myNavbar");
    if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        navbar.className = "w3-bar" + " w3-card" + " w3-animate-top" + " w3-white";
    } else {
        navbar.className = navbar.className.replace(" w3-card w3-animate-top w3-white", "");
    }
}

// Used to toggle the menu on small screens when clicking on the menu button
function toggleFunction() {
    var x = document.getElementById("navDemo");
    if (x.className.indexOf("w3-show") == -1) {
        x.className += " w3-show";
    } else {
        x.className = x.className.replace(" w3-show", "");
    }
}

</script>

<script type="text/javascript">
window.onload = function () {
  var chart = new CanvasJS.Chart("chartContainer",
  {
    title:{
      text: "Token Info"
    },
    legend: {
      maxWidth: 1200,
      itemWidth: 200
    },
    data: [
    {
      type: "pie",
      showInLegend: true,
      legendText: "{indexLabel}",
      dataPoints: [
        { y: 1000, indexLabel: "Total Supply" },
        { y: 380, indexLabel: "Uniswap Liqudity"},

        { y: 400, indexLabel: "Presale" },
        { y: 80, indexLabel: "Team Tokens" },
        { y: 30, indexLabel: "Marketing"},

      ]
    }
    ]
  });
  chart.render();
}
</script>

</body>
</html>
