<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Theme Made By www.w3schools.com -->
  <title>QR CODE GENERATOR</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
  <link href="https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet" type="text/css">
  <link href="https://fonts.googleapis.com/css?family=Lato" rel="stylesheet" type="text/css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
  <style>
  #pic {
	align: center;
  }
  
  #nest      {
	
		font-family: Lato, sans-serif;
		background-color: 	#ff6600;
		}
  
  body {
    font: 400 15px Lato, sans-serif;
    line-height: 1.8;
    color: #818181;
  }
  h2 {
    font-size: 24px;
    text-transform: uppercase;
    color: #303030;
    font-weight: 600;
    margin-bottom: 30px;
  }
  h4 {
    font-size: 19px;
    line-height: 1.375em;
    color: #303030;
    font-weight: 400;
    margin-bottom: 30px;
  }  
  .jumbotron {
    background-color: #f4511e;
    color: #fff;
    padding: 100px 25px;
    font-family: Montserrat, sans-serif;
  }
  .container-fluid {
    padding: 60px 50px;
  }
  .bg-grey {
    background-color: #f6f6f6;
  }
  .logo-small {
    color: #f4511e;
    font-size: 50px;
  }
  .logo {
    color: #f4511e;
    font-size: 200px;
  }
  .thumbnail {
    padding: 0 0 15px 0;
    border: none;
    border-radius: 0;
  }
  .thumbnail img {
    width: 100%;
    height: 100%;
    margin-bottom: 10px;
  }
  .carousel-control.right, .carousel-control.left {
    background-image: none;
    color: #f4511e;
  }
  .carousel-indicators li {
    border-color: #f4511e;
  }
  .carousel-indicators li.active {
    background-color: #f4511e;
  }
  .item h4 {
    font-size: 19px;
    line-height: 1.375em;
    font-weight: 400;
    font-style: italic;
    margin: 70px 0;
  }
  .item span {
    font-style: normal;
  }
  .panel {
    border: 1px solid #f4511e; 
    border-radius:0 !important;
    transition: box-shadow 0.5s;
  }
  .panel:hover {
    box-shadow: 5px 0px 40px rgba(0,0,0, .2);
  }
  .panel-footer .btn:hover {
    border: 1px solid #f4511e;
    background-color: #fff !important;
    color: #f4511e;
  }
  .panel-heading {
    color: #fff !important;
    background-color: #f4511e !important;
    padding: 25px;
    border-bottom: 1px solid transparent;
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
  }
  .panel-footer {
    background-color: white !important;
  }
  .panel-footer h3 {
    font-size: 32px;
  }
  .panel-footer h4 {
    color: #aaa;
    font-size: 14px;
  }
  .panel-footer .btn {
    margin: 15px 0;
    background-color: #f4511e;
    color: #fff;
  }
  .navbar {
    margin-bottom: 0;
    background-color: #f4511e;
    z-index: 9999;
    border: 0;
    font-size: 12px !important;
    line-height: 1.42857143 !important;
    letter-spacing: 4px;
    border-radius: 0;
    font-family: Montserrat, sans-serif;
  }
  .navbar li a, .navbar .navbar-brand {
    color: #fff !important;
  }
  .navbar-nav li a:hover, .navbar-nav li.active a {
    color: #f4511e !important;
    background-color: #fff !important;
  }
  .navbar-default .navbar-toggle {
    border-color: transparent;
    color: #fff !important;
  }
  footer .glyphicon {
    font-size: 20px;
    margin-bottom: 20px;
    color: #f4511e;
  }
  .slideanim {visibility:hidden;}
  .slide {
    animation-name: slide;
    -webkit-animation-name: slide;
    animation-duration: 1s;
    -webkit-animation-duration: 1s;
    visibility: visible;
  }
  @keyframes slide {
    0% {
      opacity: 0;
      transform: translateY(70%);
    } 
    100% {
      opacity: 1;
      transform: translateY(0%);
    }
  }
  @-webkit-keyframes slide {
    0% {
      opacity: 0;
      -webkit-transform: translateY(70%);
    } 
    100% {
      opacity: 1;
      -webkit-transform: translateY(0%);
    }
  }
  @media screen and (max-width: 768px) {
    .col-sm-4 {
      text-align: center;
      margin: 25px 0;
    }
    .btn-lg {
      width: 100%;
      margin-bottom: 35px;
    }
  }
  @media screen and (max-width: 480px) {
    .logo {
      font-size: 150px;
    }
  }
  </style>
</head>
<body id="myPage" data-spy="scroll" data-target=".navbar" data-offset="60">

<nav class="navbar navbar-default navbar-fixed-top">
  <div class="container">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>                        
      </button>
      <a class="navbar-brand" href="#myPage">QR CODE GENERATOR</a>
    </div>
    <div class="collapse navbar-collapse" id="myNavbar">
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#about">ABOUT US</a></li>
        <li><a href="#services">SERVICES</a></li>
		<li><a href="#portfolio">WORK</a></li>
        <li><a href="#pricing">PRICING</a></li>
        <li><a href="#contact">CONTACT</a></li>
      </ul>
    </div>
  </div>
</nav>


div id="myCarousel" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#myCarousel" data-slide-to="1"></li>
      <li data-target="#myCarousel" data-slide-to="2"></li>
    </ol>

    <!-- Wrapper for slides -->
    <div id="pic" class="carousel-inner" role="listbox">
      <div class="item active">
        <img src="http://c2.peakpx.com/wallpaper/761/157/140/qr-code-quick-response-code-scanning-wallpaper.jpg" alt="New York" align="center" width="1550" height="1000">
        <div class="carousel-caption">
          <h3>Office</h3>
          <p>Daily use of QRCodes, which makes our life easy</p>
        </div>      
      </div>
    </div>
</div>


<!-- Container (About Section) -->
<div id="about" class="container-fluid">
  <div class="row">
    <div class="col-sm-8">
      <h2>About Us</h2><br>
      <h3>The <strong>Free QR Code Generator</strong> for High Quality QR Codes</h3>
<h4>QRCode generator is one of the most popular free online qr code generators with millions of already created QR codes. The high resolution of the QR codes and the powerful design options make it one of the best free QR code generators on the web that can be used for commercial and print purposes.</h4><br>
      <h5><strong>-> Endless lifetime with unlimited scans.</strong></h5>
	  <h5><strong>-> QR Codes with Logo</strong></h5>
	  <h5><strong>-> Custom Design and Colors</strong></h5>
	  <h5><strong>-> High resolution QR Codes for Print</strong></h5>
	  <h5><strong>-> QR Code Vector Formats</strong></h5>
	  <h5><strong>-> Free for commercial usage</strong></h5>
      <br><button class="btn btn-default btn-lg">Get in Touch</button>
    </div>
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-signal logo"></span>
    </div>
  </div>
</div>

<div class="container-fluid bg-grey">
  <div class="row">
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-globe logo slideanim"></span>
    </div>
    <div class="col-sm-8">
      <h2>Our Values</h2><br>
      <h4><strong>
Set QR Content</strong><br/> Select a content type at the top for your QR code (URL, Text, Email...). After selecting your type you will see all available options. Enter all fields that should appear when scanning your QR code. Make sure everything you enter is correct because you can’t change the content once your QR code is printed.</h4><br>
     <h4><strong>Customize Design</strong><br/>You want your QR code to look unique? Set a custom color and replace the standard shapes of your QR code. The corner elements and the body can be customized individually. Add a logo to your QR code. Select it from the gallery or upload your own logo image. You can also start with one of the templates from the template gallery.</h4><br/>
    <h4><strong>
Generate QR Code</strong><br/>Set the pixel resolution of your QR code with the slider. Click the "Create QR Code"-button to see your qr code preview. Please make sure your QR code is working correctly by scanning the preview with your QR Code scanner. Use a high resolution setting if you want to get a png code with print quality.</h4><br/>
	<h4><strong>
Download Image</strong><br/>Now you can download the image files for your QR code as .png or .svg, .pdf, .eps vector graphic. If you want a vector format with the complete design please choose .svg. SVG is working in software like Adobe Illustrator or Inkscape. The logo and design settings currently only work for .png and .svg files.</h4><br/> 
  </div>
  </div>
</div>

<!-- Container (Services Section) -->
<div id="services" class="container-fluid text-center">
  <h2>SERVICES</h2>
  <h4>What we offer</h4>
  <br>
  <div class="row slideanim">
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-off logo-small"></span>
      <h4>POWER</h4>
      <p>Genarate QRCodes for boost up the influence.</p>
    </div>
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-heart logo-small"></span>
      <h4>LOVE</h4>
      <p>With our love.We provide you the QRCodes done.</p>
    </div>
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-lock logo-small"></span>
      <h4>JOB DONE</h4>
      <p>On time work.</p>
    </div>
  </div>
  <br><br>
  <div class="row slideanim">
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-leaf logo-small"></span>
      <h4>PRODUCTIVE</h4>
      <p>We believe in productive working.</p>
    </div>
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-certificate logo-small"></span>
      <h4>VERIFIED</h4>
      <p>Our QRCodes are verified.</p>
    </div>
    <div class="col-sm-4">
      <span class="glyphicon glyphicon-wrench logo-small"></span>
      <h4 style="color:#303030;">HARD WORK</h4>
      <p>Through our hard work, we meet the customer satisfaction.</p>
    </div>
  </div>
</div>






<div id="nest">
<form>

<h2 id="personal" align="center"><strong>PERSONAL INFORMATION</h2>

<div class="form-group">
    <label for="InputUrl">Enter URL</label>
    <input type="email" class="form-control" id="InputUrl" aria-describedby="UrlHelp" placeholder="Enter email">
  </div>
  
  <div class="form-group">
    <label for="InputEmail1">Enter Email address</label>
    <input type="email" class="form-control" id="InputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
    <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
  </div>
  
  <div class="form-group">
    <label for="Inputemail">Contact Number</label>
    <input type="email" class="form-control" id="InputEmail1" aria-describedby="contactHelp" placeholder="+91xxxxxxxx">
    <small id="contactHelp" class="form-text text-muted">We'll never share your number with anyone else.</small>
  </div>
  
  <div class="form-group">
    <label for="Textarea">Enter Your Text</label>
    <textarea class="form-control" id="Textarea" rows="5" placeholder="Enter your text here"></textarea>
  </div>
  
  <br />
	  
	  <hr width=1550px>
	  <br/>
  
  <h2 align="center" id="personal"><strong>SET COLOURS</h2>
  
   <fieldset class="form-group">
    <div class="form-check">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optionsRadios" id="optionsRadios1" value="option1" checked>
        Single Colour
      </label>
    </div>
	
	<div class="form-group">
    <label for="InputEmail1">Enter Colour</label>
    <input type="name" class="form-control" id="InputColor" aria-describedby="colorHelp" placeholder="E.g. Red">
  </div>
	
	  <fieldset class="form-group">
    <div class="form-check">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optionsRadios" id="optionsRadios1" value="option1" checked>
        Colour Gradient
      </label>
    </div>
	
	<div class="form-group">
    <label for="InputEmail1">Enter Primary Colour</label>
    <input type="name" class="form-control" id="InputColor" aria-describedby="colorHelp" placeholder="E.g. Red">
  </div>
	
	<div class="form-group">
    <label for="InputEmail1">Enter Gradient Colour</label>
    <input type="name" class="form-control" id="InputColor" aria-describedby="colorHelp" placeholder="E.g. Blue">
  </div>
	
	 <br />
	  
	  <hr width=1550px>
	  <br/>
	  
	  <h2 align="center" id="personal"><strong>SOCIAL CONTACT</h2>
	
	<div class="form-group">
    <label for="Inputadd">Facebook</label>
    <input type="email" class="form-control" id="Inputadd" aria-describedby="emailHelp">
  </div>
  
  <div class="form-group">
    <label for="Inputadd">Instagram</label>
    <input type="email" class="form-control" id="Inputadd" aria-describedby="emailHelp">
  </div>
  
  <div class="form-group">
    <label for="Inputadd">Twitter</label>
    <input type="email" class="form-control" id="Inputadd" aria-describedby="emailHelp">
  </div>
  
   <br />
	  
	  <hr width=1550px>
	  <br/>
	
	<h2 align="center" id="personal"><strong>QR CODE TYPE</h2>
	
  <div class="form-group">
    <label for="exampleSelect1">Image Quality</label>
    <select class="form-control" id="exampleSelect1">
      <option>Low - upto 7% data loss</option>
      <option>Medium - upto 15% data loss</option>
      <option>Quarter - upto 25% data loss</option>
      <option>upto 30% data loss</option>
    </select>
  </div>
  
  <div class="form-group">
    <label for="exampleSelect2">Image Size</label>
    <select class="form-control" id="exampleSelect2">
      <option>Smallest - 100*100 pixels</option>
      <option>Small - 200*200 pixels</option>
      <option>Medium - 300*300 pixels</option>
      <option>High - 400*400 pixels</option>
	  <option>Massive - 500*500 pixels</option>
    </select>
  </div>
  
  <div class="form-check">
    <label class="form-check-label">
      <input type="checkbox" class="form-check-input">
      I agree the Terms and Conditions.
    </label>
  </div>
  <br/>
 
  <button type="submit" class="btn btn-primary">Generate</button>

   <button type="reset" class="btn btn-primary">Reset</button><br/><br/>
</form>
</div>






<!-- Container (Portfolio Section) -->
<div id="portfolio" class="container-fluid text-center bg-grey">
  <h2>Its our work</h2><br>
  <h4>What we have created</h4>
  <div class="row text-center slideanim">
    <div class="col-sm-4">
      <div class="thumbnail">
        <img src="https://www.qrcode-monkey.com/img/qr/templates/facebook.svg" alt="Paris" width="200" height="150">
        <p><strong>Facebook QRCode</strong></p>
        <p>Yes, we build this</p>
      </div>
    </div>
    <div class="col-sm-4">
      <div class="thumbnail">
        <img src="https://www.qrcode-monkey.com/img/qr/templates/youtube.svg" alt="New York" width="200" height="150">
        <p><strong>Youtube QRCode</strong></p>
        <p>We love to make your Youtube links into QRCode</p>
      </div>
    </div>
    <div class="col-sm-4">
      <div class="thumbnail">
        <img src="https://www.qrcode-monkey.com/img/qr/templates/twitter.svg" alt="San Francisco" width="200" height="150">
        <p><strong>Twitter QRCode</strong></p>
        <p>Its our pride we do this</p>
      </div>
    </div>
  </div><br>
  
  <div id="myCarousel" class="carousel slide text-center" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#myCarousel" data-slide-to="1"></li>
      <li data-target="#myCarousel" data-slide-to="2"></li>
    </ol>

<!-- Container (Pricing Section) -->
<div id="pricing" class="container-fluid">
  <div class="text-center">
    <h2>Pricing</h2>
    <h4>Choose a payment plan that works for you</h4>
  </div>
  <div class="row slideanim">
    <div class="col-sm-4 col-xs-12">
      <div class="panel panel-default text-center">
        <div class="panel-heading">
          <h1>Basic</h1>
        </div>
        <div class="panel-body">
          <p><strong>60</strong> basic QRCodes</p>
          <p><strong>40</strong> designer QRCodes</p>
          <p><strong>PER MONTH</strong></p>
        </div>
        <div class="panel-footer">
          <h3>INR 400</h3>
          <h4>per month</h4>
          <button class="btn btn-lg">Sign Up</button>
        </div>
      </div>      
    </div>     
    <div class="col-sm-4 col-xs-12">
      <div class="panel panel-default text-center">
        <div class="panel-heading">
          <h1>Pro</h1>
        </div>
        <div class="panel-body">
         <p><strong>120</strong> basic QRCodes</p>
          <p><strong>80</strong> designer QRCodes</p>
          <p><strong>PER MONTH</strong></p>
        </div>
        <div class="panel-footer">
          <h3>INR 700</h3>
          <h4>per month</h4>
          <button class="btn btn-lg">Sign Up</button>
        </div>
      </div>      
    </div>       
    <div class="col-sm-4 col-xs-12">
      <div class="panel panel-default text-center">
        <div class="panel-heading">
          <h1>Premium</h1>
        </div>
        <div class="panel-body">
          <p><strong>180</strong> basic QRCodes</p>
          <p><strong>120</strong> designer QRCodes</p>
          <p><strong>PER MONTH</strong></p>
        </div>
        <div class="panel-footer">
          <h3>INR 1100</h3>
          <h4>per month</h4>
          <button class="btn btn-lg">Sign Up</button>
        </div>
      </div>      
    </div>    
  </div>
</div>

<div class="jumbotron text-center">
  <h1></h1> 
  <p>We specialize in QR Codes</p> 
  <form>
    <div class="input-group">
      <input type="email" class="form-control" size="50" placeholder="Email Address" required>
      <div class="input-group-btn">
        <button type="button" class="btn btn-danger">Subscribe</button>
      </div>
    </div>
  </form>
</div>

<!-- Container (Contact Section) -->
<div id="contact" class="container-fluid bg-grey">
  <h2 class="text-center">CONTACT</h2>
  <div class="row">
    <div class="col-sm-5">
      <p>Contact us and we'll get back to you within 24 hours.</p>
      <p><span class="glyphicon glyphicon-map-marker"></span> Kolkata, India</p>
      <p><span class="glyphicon glyphicon-phone"></span> +91 8250152583</p>
      <p><span class="glyphicon glyphicon-envelope"></span> fscsubhadeep02@gmail.com</p>
    </div>
    <div class="col-sm-7 slideanim">
      <div class="row">
        <div class="col-sm-6 form-group">
          <input class="form-control" id="name" name="name" placeholder="Name" type="text" required>
        </div>
        <div class="col-sm-6 form-group">
          <input class="form-control" id="email" name="email" placeholder="Email" type="email" required>
        </div>
      </div>
      <textarea class="form-control" id="comments" name="comments" placeholder="Comment" rows="5"></textarea><br>
      <div class="row">
        <div class="col-sm-12 form-group">
          <button class="btn btn-default pull-right" type="submit">Send</button>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Image of location/map -->
<img src="https://www.w3schools.com/w3images/map.jpg" class="w3-image w3-greyscale-min" style="width:100%">

<footer class="container-fluid text-center">
  <a href="#myPage" title="To Top">
    <span class="glyphicon glyphicon-chevron-up"></span>
  </a>
  <p>Designed and developed by Subhadeep Mondal</p>
</footer>

<script>
$(document).ready(function(){
  // Add smooth scrolling to all links in navbar + footer link
  $(".navbar a, footer a[href='#myPage']").on('click', function(event) {
    // Make sure this.hash has a value before overriding default behavior
    if (this.hash !== "") {
      // Prevent default anchor click behavior
      event.preventDefault();

      // Store hash
      var hash = this.hash;

      // Using jQuery's animate() method to add smooth page scroll
      // The optional number (900) specifies the number of milliseconds it takes to scroll to the specified area
      $('html, body').animate({
        scrollTop: $(hash).offset().top
      }, 900, function(){
   
        // Add hash (#) to URL when done scrolling (default click behavior)
        window.location.hash = hash;
      });
    } // End if
  });
  
  $(window).scroll(function() {
    $(".slideanim").each(function(){
      var pos = $(this).offset().top;

      var winTop = $(window).scrollTop();
        if (pos < winTop + 600) {
          $(this).addClass("slide");
        }
    });
  });
})
</script>

</body>
</html>
