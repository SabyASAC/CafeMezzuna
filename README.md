
<html>
<title> Cafe Mezzuna </title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>
body, html {
  height: 100%;
  font-family: "Calibri", sans-serif;
}

.bgimg {
  background-position: center;
  background-size: cover;
 
  min-height: 75%;
}

.menu {
  display: none;
}
</style>
<body>

<!-- Links (sit on top) -->
<div class="w3-top">
  <div class="w3-row w3-padding w3-black">
    <div class="w3-col s3">
      <a href="#" class="w3-button w3-block w3-grey">HOME</a>
    </div>
    <div class="w3-col s3">
      <a href="#about" class="w3-button w3-block w3-grey">ABOUT</a>
    </div>
    <div class="w3-col s3">
      <a href="#menu" class="w3-button w3-block w3-grey">MENU</a>
    </div>
    <div class="w3-col s3">
      <a href="#where" class="w3-button w3-block w3-grey">WHERE</a>
    </div>
  </div>
</div>

<!-- Header with image -->
<header class="bgimg w3-display-container w3-grayscale-min" id="home">
  <div class="w3-display-bottomleft w3-center w3-padding-large w3-hide-small">
    <span class="w3-tag">Open from 10 am to 8 pm </span>
  </div>
  <div class="w3-display-middle w3-center">
    <span class="w3-text-white" style="font-size:90px">Cafe<br>Mezzuna</span>
  </div>
  <div class="w3-display-bottomright w3-center w3-padding-large">
    <span class="w3-text-grey"></span>
  </div>
</header>

<!-- Add a background color and large text to the whole page -->
<div class="w3-sand w3-grayscale w3-large">

<!-- About Container -->
<div class="w3-container" id="about">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-64"><span class="w3-tag w3-wide">About The Cafe : </span></h5>
    <p> Cafe Mezzuna was founded by Anjan Chatterjee in Pune at its first outlet , followed by a branch opening in kolkata at 2014 and in bengaluru at 2015 . </p>
    
    <div class="w3-panel w3-leftbar w3-light-grey">
      <p><i>" You don't need a silver fork to eat good food"</i></p>
      <p>Owner: Speciality Restraunts Limited </p>
    </div>
   
    <p><strong>Opening hours:</strong>10 am to 8 pm </p>
    <p><strong>Address :</strong> 4th Floor, Forum Mall, Elgin Road, Kolkata </p>
  </div>
</div>

<!-- Menu Container -->
<div class="w3-container" id="menu">
  <div class="w3-content" style="max-width:700px">
 
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">THE MENU</span></h5>
  
    <div class="w3-row w3-center w3-card w3-padding">
      <a href="javascript:void(0)" onclick="openMenu(event, 'Regular');" id="myLink">
        <div class="w3-col s6 tablink">Regular</div>
      </a>
      <a href="javascript:void(0)" onclick="openMenu(event, 'Premium');">
        <div class="w3-col s6 tablink">Premium</div>
      </a>
    </div>

    <div id="Eat" class="w3-container menu w3-padding-48 w3-card">
      <h5>Captain Morgan Original     </h5>
      
      <h5>Smirnoff   </h5>
      
      <h5>Bacardi Carta Blanca   </h5>
      
      <h5>Antiguity Blue</h5>
      <p class="w3-text-grey">Scrambled eggs, roasted red pepper and garlic, with green onions 7.50</p><br>
    
      <h5>Black & White</h5>
      
    </div>

    <div id="Premium" class="w3-container menu w3-padding-48 w3-card">
      <h5>Don Alejandro</h5>
      
    
      <h5>Baileys Irish Cream </h5>
      
    
      <h5>Cointreau</h5>
      
    
      <h5>Jagermeister</h5>
      
    </div>  
    
  </div>
</div>

<!-- Contact/Area Container -->
<div class="w3-container" id="where" style="padding-bottom:32px;">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">WHERE TO FIND US</span></h5>
    <p>Find us at the above mentioned address </p>
 
    
    <p><strong>Reserve</strong> a table, ask for today's special or just send us a message:</p>
   
 Send your responses <a href="https://forms.gle/1kMhg7TFfXXP7ret8">here!</a>
  </div>
</div>

<!-- End page content -->
</div>

<script>
// Tabbed Menu
function openMenu(evt, menuName) {
  var i, x, tablinks;
  x = document.getElementsByClassName("menu");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < x.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" w3-dark-grey", "");
  }
  document.getElementById(menuName).style.display = "block";
  evt.currentTarget.firstElementChild.className += " w3-dark-grey";
}
document.getElementById("myLink").click();
</script>

 
