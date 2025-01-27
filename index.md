<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="style.css" rel="stylesheet">
    <link href="header-styles.css" rel="stylesheet">
    <link href="reservation-styles.css" rel="stylesheet">
    <link href="room-and-rates-styles.css" rel="stylesheet">
    <link href="facilities-styles.css" rel="stylesheet">
    <link href="testimonial-styles.css" rel="stylesheet">
    <link href="contact-styles.css" rel="stylesheet">
    <link href="footer-styles.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,300;1,400;1,500;1,800&display=swap" rel="stylesheet">
    <script src="https://use.fontawesome.com/e923525cb0.js"></script>
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">


<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js" integrity="sha384-OgVRvuATP1z7JjHLkuOU7Xw704+h835Lr+6QL9UvYjZE3Ipu6Tp75j7Bh/kR0JKI" crossorigin="anonymous"></script>
<script>
    // Initialize and add the map
    function initMap() {
      // The location of Amadi
      var amadi = {lat: 4.795584,lng: 7.028560 };
      // The map, centered at Amadi
      var map = new google.maps.Map(
          document.getElementById('map'), {zoom: 10, center: amadi});
      // The marker, positioned at Amadi
      var marker = new google.maps.Marker({position: amadi, map: map});
    }
        </script>
        <script async defer src="https://maps.googleapis.com/maps/api/js?key=AIzaSyD-Q_Pxh_VJZBViMKVbp9jkZprcSVi2KIg&callback=initMap">
 </script>  
<title>Hotel Landing Page</title>
</head>

<body>
    <header class="fixed-top">
        
        <nav class="hotel-navbar navbar navbar-expand-sm ">
   
            <a class="navbar-brand"  href="#">
              <img class="navbar-brand-image" src="./Resources/t-hotel-logo.png" alt="logo" >
            </a>
            <button class="navbar-toggler navbar-dark" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon">   
                    <i class="fa fa-bars" style="color:#fff; font-size:28px;"></i>
                </span>
            </button>
             
             
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
     
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link" href="#home">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#pricing">Rooms and Rates</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#facilities">Facilities</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#contact">Contact Us</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#footer">Gallery</a>
              </li>
            </ul>
              </div>
            </nav>



      </header>

<!-- Carousel -->

<div id="home"  class="hotel-carousel carousel slide" data-ride="carousel">
    <ul class="carousel-indicators">
      <li data-target="#home" data-slide-to="0" class="active"></li>
      <li data-target="#home" data-slide-to="1"></li>
      <li data-target="#home" data-slide-to="2"></li>
  
    </ul>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="./Resources/t-hotel-carousel-1.png" alt="Bed 1" width="1100px" height="500px">
        <div class="carousel-caption">
            <h1>EXPLORE OUR ROOMS</h1>
            <button type="button" class="btn btn-info">BOOK NOW</button>
        </div>   
      </div>

    </div>
    <a class="carousel-control-prev" href="#home" data-slide="prev">
      <span class="carousel-control-prev-icon"></span>
    </a>
    <a class="carousel-control-next" href="#home" data-slide="next">
      <span class="carousel-control-next-icon"></span>
    </a>
  
</div>
   
<!-- RESERVATION SECTION -->

      <section class="reservation-box container-fluid">

         <div class="reservation-box-header row"> RESERVATION </div> 
  
         <div class="reserve-form form-row">
        
        <div class="form-group col-sm-6 col-md-2">    
            <label for="date">Check in</label>
            <input class="form-control" type="date" name="date" id="date">
         </div>
         
         <div class="form-group col-sm-5  col-md-1">
            <label for="nights">Nights</label>
                <select class="custom-select" name="nights" id="nights" >
                <option value="one">1</option>
                <option value="two">2</option>
                <option value="three">3</option>
                <option value="four">4</option>
                </select>
            </div>
              
              
            <div class="form-group col-sm-6 col-md-2">
                <label for="date">Check Out</label>
                <input type="date" class="form-control" name="date" id="date">
            </div>
   
            <div class="form-group col-sm-5 col-md-1">
                <label for="adults">Adults</label>
                <select class="custom-select" name="adults" id="adults" >
                <option value="one">1</option>
                <option value="two">2</option>
                <option value="three">3</option>
                <option value="four">4</option>
                </select>
            </div>
            
            <div class="form-group col-sm-11 col-md-1">
            <label for="children" >Children</label>
            <select name="children" id="children" class="custom-select" >
                <option value="one">1</option>
                <option value="two">2</option>
                <option value="three">3</option>
                <option value="four">4</option>
            </select>
            </div>

            <div class="reserve-button form-group col-md-4">
                <button type="button" class="btn btn-info">
                CHECK AVAILABILITY</button>
            </div>
         
  
  
            </div>

 
      </section>
 

      <!-- PRICING SECTION -->

      <section id="pricing" class="pricing container-fluid">
<div class=" room-rates-header row"> 
<span class="col-1"> </span> <h1 class="col-md-10"> ROOMS AND RATES</h1>
      <span class="col-md-1">
        <a href="#pricing"><div class="header-arrow"><img src="Resources/left-arrow.svg"></div></a>
          
        <a href="#pricing"><div class="header-arrow"><img  src="Resources/right-arrow.svg"></div></a>
          </span>
    </div>
 
    <p class="room-rates-intro row">All rooms are equipped with Free Wi-Fi, an LED Smart-TV,
        21 Exciting Channels and Central Air-Conditioning.
    </p>

 
<div class="room-rates-collection  row">
    <div class="room-rates-view container col-lg-6" >  
        <div class="row">
            <img class="img-fluid rounded " src="./Resources/unsplash-bed1.png" alt="roon view 1">
        </div>
        <div class="room-rates-view-text row">
            <p>Deluxe rooms - one king bed
                <br><span class="font-weight-bold">₦10,000</span>
                <br><span style="font-size:12px"><a style="text-decoration:none;color:inherit"href="#pricing">Check Details</a> &nbsp; →</span>
            </p>  
        </div>  
          
        </div>
     
   <div class="room-rates-view container col-lg-6"> 
    <div class="row">
        <img class="img-fluid rounded" src="./Resources/unsplash-bed2.png" alt="room view 2">
    </div>   
    <div class="room-rates-view-text row"> 
        <p >Standard rooms - one king sized bed
            <br><span  class="font-weight-bold">₦20,000</span>
            <br><span style="font-size:12px"><a style="text-decoration:none;color:inherit"href="#pricing">Check Details</a> &nbsp; →</span>
        </p> 
    </div>
     
   </div>
    </div>

    

      </section>


<!-- OFFERS SECTION -->
   
<section id="facilities" class="facilities container-fluid">
<div class="facilities-header row">

    <h1>FACILITIES</h1>
</div>
 
<div class="facilities-page img-fluid container-fluid" >
    <div class="facilities-blue-overlay"></div>
    <div class="facilities-image-row row">
        <div class="facilities-image ">
            <img class="img-fluid" src="Resources/cocktail 1.png">
            <h1>Bar</h1>
        </div>
        <div class="facilities-image ">
             <img class="img-fluid "  src="Resources/restaurant.png">
             <h1>Restaurants</h1>
        </div>
        <div class="facilities-image ">
            <img class="img-fluid" src="Resources/Pool.png">
            <h1>Pool</h1>
        </div>
    
   
        <div class="facilities-image  " >
            <img class="img-fluid"  src="Resources/spa 1.png">
            <h1>Spa/Wellness</h1>
        </div>
        <div class="facilities-image  "> 
            <img class="img-fluid" src="Resources/cinema 1.png">
            <h1>Cinema</h1>
        </div>
        <div class="facilities-image ">
             <img class="img-fluid" src="Resources/Wi-fi.png">
             <h1>Wi-Fi</h1>
        </div>

    </div>
   
</div>

</section>

<!-- TESTIMONIALS SECTION -->
<section class="testimonials container-fluid">

    <div class="testimonials-header row"> 
        <span class="col-md-1"> </span>  <h1 class=" col-md-10">TESTIMONIALS</h1> <span class="col-md-1">
                <a href="#pricing"><div class="header-arrow"><img src="Resources/left-arrow.svg"></div></a>
                  
                <a href="#pricing"><div class="header-arrow"><img  src="Resources/right-arrow.svg"></div></a>
                  </span>
    </div>
    <div class="testimonials-list row">
        <div class="testimonials-item col-md-5">
            <img class="rounded-circle" src="./Resources/avatar1.png" alt="avatar">
            <p>T Hotel is a home away from home, it has a serene
                environment, 24 hours power supply, free Wi-fi and 
                the Facilities are top-notch.
                <span>Innocent Tamunosiki, Traveller</span>
            </p>
        </div>
      

    </div>

    

    

</section>


<!-- CONTACT US SECTION -->

<section id="contact" class="contact container-fluid">
    <div class="contact-header row">
        <span class="col-md-3"></span>
        <h1>Contact Us</h1>
    </div>
    <div class="contact-body row">
        <div id="map" class="map col-sm-5">
             <!--The div element for the map -->      
        </div>
        <div class="contact-form col-sm-5">
            <div class="form-group ">    
             <input class="form-control" placeholder="Name" type="text" name="name" id="name">
             <input class="form-control" placeholder="Email" type="email" name="email" id="email">
             <textarea class="form-control" placeholder="Leave a note" type="text" name="comments" id="comments"></textarea>
             <button class="btn-info" type="submit">Send</button>
             </div>
           
        </div>
       
    </div>
  
</section>

<!-- FOOTER SECTION -->

<section id="footer" class="footer container-fluid">

    <div class="footer-logo row">
        <img src="./Resources/Logo3d.svg">
    </div>
    <div class="footer-body row">

    <div class="footer-block col-md-5">
       
        
        <ul>
            <li ><h3 style="margin-left: 20px" >Book Now</h3></li>
          <div> <i class="fa pl-2 fa-map-marker  fa-lg" style="margin-right: 29px;" aria-hidden="true"></i> <li> No 11, Somaria Ama, Portharcourt, Rivers State, Nigeria</li></div> 
          <div> <i class="fa pl-2 fa-phone fa-lg" aria-hidden="true"></i> <li>+23400000000</li></div>
           <div><i class="fa pl-2 fa-envelope fa-lg" style="margin-right: 21px" aria-hidden="true"></i> <li>innocenttamunosiki@gmail.com</li></div>
        </ul>
    </div>
    <div class="footer-block col-md">
        <ul>
            <li><h3>Customer care</h3></li>
            <li><a href="#contact">Contact Us</a></li>
            <li><a href="#pricing">Rooms and Rates</a></li>
            <li><a href="#facilites" >Facilities</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </div>
    <div class="footer-block col-md">
        <ul>
            <li><h3>Facilities</h3></li>
            <li><a href="#facilites" >Spa and Gym</a></li>
            <li><a href="#facilites" >Restaurant</a></li>
        <li><a href="#facilites" >Bar</a></li>
        <li><a href="#facilites" >Cinema</a></li>
        </ul>
    </div>


    </div>
    <div class="footer-social row">
        <div class="col-md-4">
            <a href="#"><i class="fa fa-facebook fa-lg" aria-hidden="true"></i></a>

            <a href="#"><i class="fa fa-twitter fa-lg" aria-hidden="true"></i></a>

            <a href="#"><i class="fa fa-linkedin fa-lg" aria-hidden="true"></i></a>

            <a href="#"><i class="fa fa-instagram fa-lg" aria-hidden="true"></i></a>
        </div>
      
    </div>
    

    

      
</section>
</body>

</html>
