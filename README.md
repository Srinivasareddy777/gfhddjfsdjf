<!--Log in page-->
<!doctype html>
<html>
<head>
<link rel="stylesheet" href="css1.css">
<script>
var objPeople = [
{
	username:"srinivas",
        password:"123"
},
{
	username:"srikanth",
        password:"123"
},
{
	username:"saicharan",
        password:"123"
},
{
	username:"vivek",
        password:"123"
}
]
function getInfo(){
var username=document.getElementById("username").value
var password=document.getElementById("password").value
var f=0
for(i=0;i<objPeople.length;i++)
{
	if(username==objPeople[i].username && password==objPeople[i].password)
        {
       alert(username+"  is logged in");
       window.location.href="main page.html";
       return
      }
        else
        {
	  f=1
        }     
}
if(f==1)
{
alert("INVALID USER ID OR PASSWORD");

}
}</script>

</head>

<body>
<background:spaghetti.jpg; backgroung-repeat:norepeat; background-size:100%; >
<div class="loginbox">
<img src="avatar1.png" class="avatar">
<form>
<h1>LOGIN HERE</h1>
<p>USERNAME</p>
<input id="username" type="text" name="" placeholder="Enter Username" required>
<p>PASSWORD</p>
<input id="password" type="password" name="" placeholder="Enter Password" required>
</form>
<input type="submit" onclick="getInfo()" name="" value="login">
<p>Don't have an account?<a href="register form.html">Signup</a></p>
</body>
</html>


<!--Signup-->
<!doctype html>
<html>
<head>
<title> Signup Form </title>
<style>
body{
	margin:0;
	background-image:url(redchilli.jpg);
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	}
header{
	background:;
	color:white;
	paddings:15px 0px 6px 40px;
	height:80px;
	opacity:0.7;
	}
	
	p{
		color: white;
		 text-align: center;
			    font-size: x-large;
			    font-weight: 600;
			    font-style: italic;
	}
header h1{
	display:inline;
	color:white;
	font-weight:400;
	font-size:40px;
	float:left;
	margin-top:15px;
	margin-right:15px;
	margin-left: 15px;
}
h2{
	color: white;
}
nav ul{
	display:inline;
	padding:0px;
	float:left;
	margin-left: 40px;
	margin-top: 20px;
	
}
nav ul li{
	display:inline-block;
	list-style-type:none;
	color:white;
	float:left;
	margin-right:40px;
	margin-top: 10px;
}
nav ul li a{
	color:white;
	font-size: 20;
	text-decoration:none;
}
.homeblack:hover{
	background-color:green;
	padding:20px 20px 22px 20px;
}
.divider{
background-color:green;
}
body{
	margin:0;
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	}

.loginbox{
    width: 400px;
    height: 700px;
    background:rgba(0,0,0,0)  ;
    color: #fff;
    top: 53%;
    left: 50%;
    position: absolute;
    transform: translate(-50%,-50%);
    box-sizing: border-box;
    padding: 70px 30px;
}
.avatar{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    position:absolute;
    top: -50px;
    left: calc(50% - 15%);
     
}
h1{
    margin:0 ;
    padding:0 0 20px;
    text-align:center;
    font-size: 22px;
}
.loginbox p{
    margin: 0;
    padding: 0;
    font-weight: bold;
}

.loginbox input{
width: 100%;
margin-bottom: 20px;
}
.loginbox input[type="text"],input[type="password"],input[type="email"],input[type="number"]
{
border: none;
    border-bottom: 1px solid #fff;
    background: transparent;
    outline: none;
    height: 40px;
    color: #fff;
    font-size: 16px; 
}
.loginbox input[type="submit"]
{
border: none;
outline: none;
height: 40px;
background: #fb2525;
color: #fff;
font-size: 18px;
border-radius: 20px;
}
.loginbox input[type="submit"]:hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}

.loginbox a{
    text text-decoration: none ;
    font-size: 12px;
    line-height: 20px;
    color:darkgrey;
}
.loginbox a:hover
{
color :#ffc107
}
</style>
<body>
 <background="redchilli.jpg" background-repeat: no-repeat; background-size:100%; >
 <header>
<nav>
   <a href="main page.html"><h1>HOME</h1></a>
   <ul  STYLE=" TOP:0px; right:200px;" >
   <li><a class="homeblack" href="about us.html">About us</a></li>
     <li><a class="homeblack" href="allrestaurants.html">Restaurants</a></li>

<li><a class="homeblack" href="extra.html">Discussions</a></li>
<li><a class="homeblack" href="remarks.html">Reviews</a></li>
<li><a class="homeblack" href="contact us.html">Contact us</a></li>
<li><a class="homeblack" href="sign up.html">Sign Up</a><li>
<li><a class="homeblack" href="project.html">Login</a><li>
</ul>
</nav>
</header>
    <div class="loginbox">
  
        <h1> Signup Here</h1>
        <form name="signup" onSubmit="return validation()"> 
        <p> Name </p>
            <input type="text" name="uname1" placeholder="First Name Last Name" required>
            <p> Email </p>
            <input type="email" name="email" placeholder="Enter email" required><br>
            <p> Username</p>
            <input type="text" name="uname" placeholder="Enter Username" required>
            <p> Password </p>
            <input type="password" name="pwd" placeholder="Enter Password" required><br>
            <p> Confirm Password </p>
            <input type="password" name="pwd1" placeholder="Confirm Password" required><br>
            <p>Mobile Number</p>
            <input type="number" name="num" placeholder="Enter Mobile Number"required ><br>
          <a>  <input type="submit" onclick="sign()" name="" value="Signup"><br></a>
            
           
            </form>
    </div>
    <!--JavaScript-->
    <script type="text/javascript">
    function validation()
        {
            var uname=document.signup.uname.value;
            var pwd=document.signup.pwd.value;
            var pwd1=document.signup.pwd1.value;
            if(uname=="" || pwd=="")
                {
                    alert("Required field are empty");
                    return;
                }
            if(uname.length<6)
                {
                    alert("UsernameMust be min 6 characters");
                      return;                                        
                }
            if(pwd.length<6 ||pwd.length>12)
                {
                    alert("Passwordmust be 6 to 12 Characters");
                      return;                                          
                }
            if(pwd!=pwd1)
               {
               alert("passwords didnt match");
              return;                                  
               }
            if(num.length!=10)
                {
                    alert("Enter Valid Mobile Number");
                }
				
				
        }
		
    </script>
    
</body>
</head>
</html>    


<!--All Restaurents-->

<!DOCTYPE html>
<html>
<head>
 <title> Restaurants</title>  
<style> 
   body{
	margin:0;
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	blur:55px;
	}
	header	background:black;
	color:white;
	paddings:15px 0px 6px 40px;
	height:80px;
	opacity:0.7;
	}
	
	p{
		color: white;
		 text-align: center;
			    font-size: x-large;
			    font-weight: 600;
			    font-style: italic;
	}
header h1{
	display:inline;
	color:white;
	font-weight:400;
	font-size:40px;
	float:left;
	margin-top:15px;
	margin-right:15px;
	margin-left: 15px;
}
h2{
	color: white;
}
nav ul{
	display:inline;
	padding:0px;
	float:left;
	margin-left: 40px;
	margin-top: 20px;
	
}
nav ul li{
	display:inline-block;
	list-style-type:none;
	color:white;
	float:left;
	margin-right:40px;
	margin-top: 10px;
}
nav ul li a{
	color:white;
	font-size: 20;
	text-decoration:none;
}
.homeblack:hover{
	background-color:green;
	padding:20px 20px 22px 20px;
}
.divider{
background-color:green;
}

.navigation{
    float: center;
    margin-right: 50px;
    margin-left: 60px;
    margin-top: 50px;
}

.navigation li{

    display: inline-block;
    margin-left: 70px;
    margin-top: -20px;
    margin-right: 20px;
    margin-bottom: -20px;
}

.navigation li a{
    color: white;
    background-color: rgba(0,0,0,0.5);
     border: 1px solid chocolate;
    border-radius: 20px;
    border-color: antiquewhite;
    text-decoration:none;
    text-transform: uppercase;
    padding: 10px;
}
.navigation li a:hover,
.navigation li a:active{
    border-bottom: solid;
    border-bottom-color: darkred;
    background-color: darkcyan;
}
body{
    margin:0;
    padding:0;
    background: url(cocktail.jpg);
    background-size: cover;
    background-position:center;
    font-family: sans-serif;
}
.container
{
    width: 90%;
    padding: 10px;
    background: rgba(0,0,0,0.5);
    margin: 100px auto;
    display: flex;
    justify-content: center;
}
.box
{
width: 250px;
height: 300px;
background: rgba(0,0,0,0.3);
  
float: left;
margin: 0px 10px;
    transition: 1s;
}
.box:hover{
    transform: scale(1.3);
    background: rgba(0,0,0,0.3);
    box-shadow: 2px 2px 2px #000;
    z-index: 2;
}
.detailsbutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 18px;
    margin-top: 30px;
    font-weight: bold;
}
.detailsbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.viewbutn
{
    text-align: center;
position: absolute;
border: black;
outline: none;
height: 25px;
width: 55px;    
background: #fb2525;
color: #fff;
font-size: 15px;
border-radius:20px;
    margin-left: 84px;
    margin-top: 30px;
    font-weight: bold;
}
.viewbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.image
{
margin-top: 30px;
border-radius: 10px;
border-color: azure

}

.menubutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 148px;
    margin-top: 30px;
    font-weight: bold;
}
.menubutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.gallerybutn
{
text-align: left;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 155px;    
background-color: dimgray;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 35px;
    margin-top: 80px;
    font-weight: bold;
}
.gallerybutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}

  </style>  
<body background="image1.jpg" background-repeat: no-repeat; background-size:100%; >
<header>
<nav>
   <a href="main page.html"><h1>HOME</h1></a>
   <ul  STYLE=" TOP:0px; right:200px;" >
   <li><a class="homeblack" href="about us.html">About us</a></li>
     <li><a class="homeblack" href="allrestaurants.html">Restaurants</a></li>

<li><a class="homeblack" href="extra.html">Discussions</a></li>
<li><a class="homeblack" href="remarks.html">Reviews
</a></li>
<li><a class="homeblack" href="contact us.html">Contact us</a></li>
<li><a class="homeblack" href="sign up.html">Sign up</a><li>
<li><a class="homeblack" href="project.html">Login</a><li>
</ul>
</nav>
</header>
               <ul class="navigation">
                   <li><a href="allrestaurants.html">All</a></li>
                   <li><a href="chennairestaurants.html">Chennai</a></li>
                   <li><a href="delhirestaurants.html">Delhi</a></li>
                   
                   
    </ul>
    
    <div class="container">
     <div class="box">
        <center><img src="absolutebarbequelogo.jpg" width="160px" height="100px" class="image"></center></a>
        <a class="detailsbutn" href="details11.html"><center>details</center></a>
        <a class="viewbutn" href="absolutebarbequeoffers.html"><center>offers</center></a>
        <a class="menubutn" href="absolutebarbequemenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="absolutebarbequeimages.html"><center>Restaurant Gallery</center></a>
        </div>
     <div class="box">
    <center><img src="dineestylogo.jpg" width="180px" height="100px" class="image"></center></a>
       <a class="detailsbutn" href="details1.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="dineestymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="dineestyimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
         <center><img src="grillboxlogo.jpg" width="160px" height="100px" class="image"></center></a>
     <a class="detailsbutn" href="details13.html"><center>details</center></a>
        <a class="viewbutn" href="grillboxoffers.html"><center>offers</center></a>
        <a class="menubutn" href="grillboxmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="grillboximages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="golasizzlerslogo.png" width="160px" height="100px" class="image"></center></a>
 <a class="detailsbutn" href="details3.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="golasizzlersmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="golasizzlersimages.html"><center>Restaurant Gallery</center></a>
    </div>
	 </div>
    <div class="container">
     <div class="box">
        <center><img src="annalakshmilogo.jpg" width="180px" height="100px" class="image"></center></a>
		  <a class="detailsbutn" href="details12.html"><center>details</center></a>
         <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="annalakshmimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="annalakshmiimages.html"><center>Restaurant Gallery</center></a></div>
		
        <div class="box">
       <center><img src="mealodramalogo.jpg" width="180px" height="100px" class="image"></center></a>
	     <a class="detailsbutn" href="details2.html"><center>details</center></a>
       <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="mealodramamenu.html"><center>Menu</center></a>
      <a class="gallerybutn" href="mealodramaimages.html"><center>Restaurant Gallery</center></a></div>  
      
        <div class="box">
         <center><img src="pindbawarchilogo.jpg" width="160px" height="100px" class="image"></center></a>
      <a class="detailsbutn" href="details4.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="pindbawarchimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="pindbawarchiimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="savorylogo.jpg" width="160px" height="100px" class="image"></center></a>
  <a class="detailsbutn" href="details14.html"><center>details</center></a>
        <a class="viewbutn" href="savoryoffers.html"><center>offers</center></a>
        <a class="menubutn" href="savorymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="savoryimages.html"><center>Restaurant Gallery</center></a>
    </div>

    </div>
	
</head>
</body>
</html>

<!--Restaurent of one place-->
<html>
<head>
 <title> Restaurants</title>  
<style> 
   body{
	margin:0;
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	blur:5px;
	}
	header{
	background:black;
	color:white;
	paddings:15px 0px 6px 40px;
	height:80px;
	opacity:0.7;
	}
	
	p{
		color: white;
		 text-align: center;
			    font-size: x-large;
			    font-weight: 600;
			    font-style: italic;
	}
header h1{
	display:inline;
	color:white;
	font-weight:400;
	font-size:40px;
	float:left;
	margin-top:15px;
	margin-right:15px;
	margin-left: 15px;
}
h2{
	color: white;
}
nav ul{
	display:inline;
	padding:0px;
	float:left;
	margin-left: 40px;
	margin-top: 20px;
	
}
nav ul li{
	display:inline-block;
	list-style-type:none;
	color:white;
	float:left;
	margin-right:40px;
	margin-top: 10px;
}
nav ul li a{
	color:white;
	font-size: 20;
	text-decoration:none;
}
.homeblack:hover{
	background-color:green;
	padding:20px 20px 22px 20px;
}
.divider{
background-color:green;
}

.navigation{
    float: center;
    margin-right: 50px;
    margin-left: 60px;
    margin-top: 50px;
}

.navigation li{
    display: inline-block;
    margin-left: 70px;
    margin-top: -20px;
    margin-right: 20px;
    margin-bottom: -20px;
}

.navigation li a{
    color: white;
    background-color: rgba(0,0,0,0.5);
     border: 1px solid chocolate;
    border-radius: 20px;
    border-color: antiquewhite;
    text-decoration:none;
    text-transform: uppercase;
    padding: 10px;
}
.navigation li a:hover,
.navigation li a:active{
    border-bottom: solid;
    border-bottom-color: darkred;
    background-color: darkcyan;
}
body{
    margin:0;
    padding:0;
    background: url(lotous.jpg);
    background-size: cover;
    background-position:center;
    font-family: sans-serif;
}
.container
{

    width: 90%;
    padding: 10px;
    background: rgba(0,0,0,0.5);
    margin: 100px auto;
    display: flex;
    justify-content: center;
}
.box
{
width: 250px;
height: 300px;
background: rgba(0,0,0,0.3);
  
float: left;
margin: 0px 10px;
    transition: 1s;
}
.box:hover{
    transform: scale(1.3);
    background: rgba(0,0,0,0.3);
    box-shadow: 2px 2px 2px #000;
    z-index: 2;
}
.viewbutn
{
    text-align: center;
position: absolute;
border: black;
outline: none;
height: 25px;
width: 55px;    
background: #fb2525;
color: #fff;
font-size: 15px;
border-radius:20px;
    margin-left: 84px;
    margin-top: 30px;
    font-weight: bold;
}
.viewbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.image
{
margin-top: 30px;
border-radius: 10px;
border-color: azure

}
.detailsbutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 18px;
    margin-top: 30px;
    font-weight: bold;
}
.detailsbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}

.menubutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 148px;
    margin-top: 30px;
    font-weight: bold;
}
.menubutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.gallerybutn
{
text-align: left;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 155px;    
background-color: dimgray;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 35px;
    margin-top: 80px;
    font-weight: bold;
}
.gallerybutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}

  </style>  
<body background="delhi.jpg" background-repeat: no-repeat; background-size:100%; >
<header>
<nav>
   <a href="main page.html"><h1>HOME</h1></a>
   <ul  STYLE=" TOP:0px; right:200px;" >
   <li><a class="homeblack" href="about us.html">About us</a></li>
         <li><a class="homeblack" href="allrestaurants.html">Restaurants</a></li>

<li><a class="homeblack" href="extra.html">Discussions</a></li>
<li><a class="homeblack" href="remarks.html">Reviews</a></li>
<li><a class="homeblack" href="contact us.html">Contact us</a></li>
<li><a class="homeblack" href="sign up.html">Sign Up</a><li>
<li><a class="homeblack" href="project.html">Login</a><li>
</ul>
</nav>
</header>
               <ul class="navigation">
                   <li><a href="allrestaurants.html">All</a></li>
				   <li><a href="delhirestaurants.html">Delhi</a></li>
                   <li><a href="chennairestaurants.html">Chennai</a></li>
                   
                   
                   
    </ul>
    <form class="loginboxhyd">
        <input type="submit" name="" value="Delhi">
    </form>
    <div class="container">
     <div class="box">
        <center><img src="dineestylogo.jpg" width="160px" height="100px" class="image"></center></a>
  <a class="detailsbutn" href="details1.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="dineestymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="dineestyimages.html"><center>Restaurant Gallery</center></a>
        </div>
     <div class="box">
    <center><img src="mealodramalogo.jpg" width="180px" height="100px" class="image"></center></a>
       <a class="detailsbutn" href="details2.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="mealodramamenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="mealodramaimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
         <center><img src="golasizzlerslogo.png" width="160px" height="100px" class="image"></center></a>
      <a class="detailsbutn" href="details3.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="golasizzlersmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="golasizzlers.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="pindbawarchilogo.jpg" width="160px" height="100px" class="image"></center></a>
<a class="detailsbutn" href="details4.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="pindbawarchimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="pindbawarchiimages.html"><center>Restaurant Gallery</center></a>
    </div>
    
  <script>
// Get the modal
var modal = document.getElementById('myModal');

// Get the button that opens the modal
var btn = document.getElementById("myBtn");

// Get the <span> element that closes the modal
var span = document.getElementsByClassName("close")[0];

// When the user clicks the button, open the modal 
btn.onclick = function() {
    modal.style.display = "block";
}

// When the user clicks on <span> (x), close the modal
span.onclick = function() {
    modal.style.display = "none";
}

// When the user clicks anywhere outside of the modal, close it
window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = "none";
    }
}
</script>
 
    
</head>
</body>
</html


<!-- Restaurent of another place-->
<html>
<head>
 <title> Restaurants</title>  
<style> 
   body{
	margin:0;
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	blur:5px;
 background-image:url("chennai.jpg");
	}
	header{
	background:black;
	color:white;
	paddings:15px 0px 6px 40px;
	height:80px;
	opacity:0.7;
	}
	
	p{
		color: white;
		 text-align: center;
			    font-size: x-large;
			    font-weight: 600;
			    font-style: italic;
	}
header h1{
	display:inline;
	color:white;
	font-weight:400;
	font-size:40px;
	float:left;
	margin-top:15px;
	margin-right:15px;
	margin-left: 15px;
}
h2{
	color: white;
}
nav ul{
	display:inline;
	padding:0px;
	float:left;
	margin-left: 40px;
	margin-top: 20px;
	
}
nav ul li{
	display:inline-block;
	list-style-type:none;
	color:white;
	float:left;
	margin-right:40px;
	margin-top: 10px;
}
nav ul li a{
	color:white;
	font-size: 20;
	text-decoration:none;
}
.homeblack:hover{
	background-color:green;
	padding:20px 20px 22px 20px;
}
.divider{
background-color:green;
}

.navigation{
    float: center;
    margin-right: 50px;
    margin-left: 60px;
    margin-top: 50px;
}

.navigation li{
    display: inline-block;
    margin-left: 70px;
    margin-top: -20px;
    margin-right: 20px;
    margin-bottom: -20px;
}

.navigation li a{
    color: white;
    background-color: rgba(0,0,0,0.5);
     border: 1px solid chocolate;
    border-radius: 20px;
    border-color: antiquewhite;
    text-decoration:none;
    text-transform: uppercase;
    padding: 10px;
}
.navigation li a:hover,
.navigation li a:active{
    border-bottom: solid;
    border-bottom-color: darkred;
    background-color: darkcyan;
}
body{
    margin:0;
    padding:0;
    background: url(chennai.jpg);
    background-size: cover;
    background-position:center;
    font-family: sans-serif;
}
.container
{
    width: 90%;
    padding: 10px;
    background: rgba(0,0,0,0.5);
    margin: 100px auto;
    display: flex;
    justify-content: center;
}
.box
{
width: 250px;
height: 300px;
background: rgba(0,0,0,0.3);
  
float: left;
margin: 0px 10px;
    transition: 1s;
}
.box:hover{
    transform: scale(1.3);
    background: rgba(0,0,0,0.3);
    box-shadow: 2px 2px 2px #000;
    z-index: 2;
}
.detailsbutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 18px;
    margin-top: 30px;
    font-weight: bold;
}
.detailsbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.viewbutn
{
    text-align: center;
position: absolute;
border: black;
outline: none;
height: 25px;
width: 55px;    
background: #fb2525;
color: #fff;
font-size: 15px;
border-radius:20px;
    margin-left: 84px;
    margin-top: 30px;
    font-weight: bold;
}
.viewbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.image
{
margin-top: 30px;
border-radius: 10px;
border-color: azure

}

.menubutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 148px;
    margin-top: 30px;
    font-weight: bold;
}
.menubutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.gallerybutn
{
text-align: left;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 155px;    
background-color: dimgray;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 35px;
    margin-top: 80px;
    font-weight: bold;
}
.gallerybutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}


  </style>  
<body >
<header>
<nav>
   <a href="main page.html"><h1>HOME</h1></a>
   <ul  STYLE=" TOP:0px; right:200px;" >
   <li><a class="homeblack" href="about us.html">About us</a></li>
         <li><a class="homeblack" href="allrestaurants.html">Restaurants</a></li>

<li><a class="homeblack" href="extra.html">Discussions</a></li>
<li><a class="homeblack" href="remarks.html">Reviews</a></li>
<li><a class="homeblack" href="contact us.html">Contact us</a></li>
<li><a class="homeblack" href="sign up.html">Sign up</a><li>
<li><a class="homeblack" href="trial.html">Login</a><li>
</ul>
</nav>
</header>
               <ul class="navigation">
                   <li><a href="allrestaurants.html">All</a></li>
                   <li><a href="chennairestaurants.html">Chennai</a></li>
                   <li><a href="delhirestaurants.html">Delhi</a></li>
                   
                   
    </ul>
    <form class="loginboxhyd">
        <input type="submit" name="" value="Chennai">
    </form>
    <div class="container">
     <div class="box">
        <center><img src="absolutebarbequelogo.jpg" width="160px" height="100px" class="image"></center></a>
         <a class="detailsbutn" href="details11.html"><center>details</center></a>
        <a class="viewbutn" href="absolutebarbequeoffers.html"><center>offers</center></a>
        <a class="menubutn" href="absolutebarbequemenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="absolutebarbequeimages.html"><center>Restaurant Gallery</center></a>
        </div>
     <div class="box">
    <center><img src="annalakshmilogo.jpg" width="180px" height="100px" class="image"></center></a>
        <a class="detailsbutn" href="details12.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="annalakshmimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="annalakshmiimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
         <center><img src="grillboxlogo.jpg" width="160px" height="100px" class="image"></center></a>
      <a class="detailsbutn" href="details13.html"><center>details</center></a>
        <a class="viewbutn" href="grillboxoffers.html"><center>offers</center></a>
        <a class="menubutn" href="grillboxmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="grillboximages"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="savorylogo.jpg" width="160px" height="100px" class="image"></center></a>
  <a class="detailsbutn" href="details14.html"><center>details</center></a>
        <a class="viewbutn" href="savoryoffers.html"><center>offers</center></a>
        <a class="menubutn" href="savorymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="savoryimages.html"><center>Restaurant Gallery</center></a>
    </div>
    
   
    
</head>
</body>
</html







<!--Home Page-->
<!DOCTYPE html>
<html>
<head>
 <title> Restaurants</title>  
<style> 
   body{
	margin:0;
	background-repeat: no-repeat fixed ; background-size:100% 100% ; background-attachment:fixed; 
	blur:55px;
	}
	header{
	background:black;
	color:white;
	paddings:15px 0px 6px 40px;
	height:80px;
	opacity:0.7;
	}
	
	p{
		color: white;
		 text-align: center;
			    font-size: x-large;
			    font-weight: 600;
			    font-style: italic;
	}
header h1{
	display:inline;
	color:white;
	font-weight:400;
	font-size:40px;
	float:left;
	margin-top:15px;
	margin-right:15px;
	margin-left: 15px;
}
h2{
	color: white;
}
nav ul{
	display:inline;
	padding:0px;
	float:left;
	margin-left: 40px;
	margin-top: 20px;
	
}
nav ul li{
	display:inline-block;
	list-style-type:none;
	color:white;
	float:left;
	margin-right:40px;
	margin-top: 10px;
}
nav ul li a{
	color:white;
	font-size: 20;
	text-decoration:none;
}
.homeblack:hover{
	background-color:green;
	padding:20px 20px 22px 20px;
}
.divider{
background-color:green;
}

.navigation{
    float: center;
    margin-right: 50px;
    margin-left: 60px;
    margin-top: 50px;
}

.navigation li{

    display: inline-block;
    margin-left: 70px;
    margin-top: -20px;
    margin-right: 20px;
    margin-bottom: -20px;
}

.navigation li a{
    color: white;
    background-color: rgba(0,0,0,0.5);
     border: 1px solid chocolate;
    border-radius: 20px;
    border-color: antiquewhite;
    text-decoration:none;
    text-transform: uppercase;
    padding: 10px;
}
.navigation li a:hover,
.navigation li a:active{
    border-bottom: solid;
    border-bottom-color: darkred;
    background-color: darkcyan;
}
body{
    margin:0;
    padding:0;
    background: url(cocktail.jpg);
    background-size: cover;
    background-position:center;
    font-family: sans-serif;
}
.container
{
    width: 90%;
    padding: 10px;
    background: rgba(0,0,0,0.5);
    margin: 100px auto;
    display: flex;
    justify-content: center;
}
.box
{
width: 250px;
height: 300px;
background: rgba(0,0,0,0.3);
  
float: left;
margin: 0px 10px;
    transition: 1s;
}
.box:hover{
    transform: scale(1.3);
    background: rgba(0,0,0,0.3);
    box-shadow: 2px 2px 2px #000;
    z-index: 2;
}
.detailsbutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 18px;
    margin-top: 30px;
    font-weight: bold;
}
.detailsbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.viewbutn
{
    text-align: center;
position: absolute;
border: black;
outline: none;
height: 25px;
width: 55px;    
background: #fb2525;
color: #fff;
font-size: 15px;
border-radius:20px;
    margin-left: 84px;
    margin-top: 30px;
    font-weight: bold;
}
.viewbutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.image
{
margin-top: 30px;
border-radius: 10px;
border-color: azure

}

.menubutn
{
    text-align: center;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 55px;    
background-color: limegreen;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 148px;
    margin-top: 30px;
    font-weight: bold;
}
.menubutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}
.gallerybutn
{
text-align: left;
position: absolute;
border-color: black;
outline: none;
height: 25px;
width: 155px;    
background-color: dimgray;
color: #fff;
font-size: 15px;
border-radius: 20px;
    margin-left: 35px;
    margin-top: 80px;
    font-weight: bold;
}
.gallerybutn :hover
{
    cursor:pointer;
    background: #ffc107;
    color: #000;
}

  </style>  
<body background="image1.jpg" background-repeat: no-repeat; background-size:100%; >
<header>
<nav>
   <a href="main page.html"><h1>HOME</h1></a>
   <ul  STYLE=" TOP:0px; right:200px;" >
   <li><a class="homeblack" href="about us.html">About us</a></li>
     <li><a class="homeblack" href="allrestaurants.html">Restaurants</a></li>

<li><a class="homeblack" href="extra.html">Discussions</a></li>
<li><a class="homeblack" href="remarks.html">Reviews
</a></li>
<li><a class="homeblack" href="contact us.html">Contact us</a></li>
<li><a class="homeblack" href="sign up.html">Sign up</a><li>
<li><a class="homeblack" href="project.html">Login</a><li>
</ul>
</nav>
</header>
               <ul class="navigation">
                   <li><a href="allrestaurants.html">All</a></li>
                   <li><a href="chennairestaurants.html">Chennai</a></li>
                   <li><a href="delhirestaurants.html">Delhi</a></li>
                   
                   
    </ul>
    
    <div class="container">
     <div class="box">
        <center><img src="absolutebarbequelogo.jpg" width="160px" height="100px" class="image"></center></a>
        <a class="detailsbutn" href="details11.html"><center>details</center></a>
        <a class="viewbutn" href="absolutebarbequeoffers.html"><center>offers</center></a>
        <a class="menubutn" href="absolutebarbequemenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="absolutebarbequeimages.html"><center>Restaurant Gallery</center></a>
        </div>
     <div class="box">
    <center><img src="dineestylogo.jpg" width="180px" height="100px" class="image"></center></a>
       <a class="detailsbutn" href="details1.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="dineestymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="dineestyimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
         <center><img src="grillboxlogo.jpg" width="160px" height="100px" class="image"></center></a>
     <a class="detailsbutn" href="details13.html"><center>details</center></a>
        <a class="viewbutn" href="grillboxoffers.html"><center>offers</center></a>
        <a class="menubutn" href="grillboxmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="grillboximages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="golasizzlerslogo.png" width="160px" height="100px" class="image"></center></a>
 <a class="detailsbutn" href="details3.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="golasizzlersmenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="golasizzlersimages.html"><center>Restaurant Gallery</center></a>
    </div>
	 </div>
    <div class="container">
     <div class="box">
        <center><img src="annalakshmilogo.jpg" width="180px" height="100px" class="image"></center></a>
		  <a class="detailsbutn" href="details12.html"><center>details</center></a>
         <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="annalakshmimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="annalakshmiimages.html"><center>Restaurant Gallery</center></a></div>
		
        <div class="box">
       <center><img src="mealodramalogo.jpg" width="180px" height="100px" class="image"></center></a>
	     <a class="detailsbutn" href="details2.html"><center>details</center></a>
       <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="mealodramamenu.html"><center>Menu</center></a>
      <a class="gallerybutn" href="mealodramaimages.html"><center>Restaurant Gallery</center></a></div>  
      
        <div class="box">
         <center><img src="pindbawarchilogo.jpg" width="160px" height="100px" class="image"></center></a>
      <a class="detailsbutn" href="details4.html"><center>details</center></a>
        <a class="viewbutn" href="#Hello"><center>offers</center></a>
        <a class="menubutn" href="pindbawarchimenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="pindbawarchiimages.html"><center>Restaurant Gallery</center></a>
    </div>
     <div class="box">
     <center><img src="savorylogo.jpg" width="160px" height="100px" class="image"></center></a>
  <a class="detailsbutn" href="details14.html"><center>details</center></a>
        <a class="viewbutn" href="savoryoffers.html"><center>offers</center></a>
        <a class="menubutn" href="savorymenu.html"><center>Menu</center></a>
        <a class="gallerybutn" href="savoryimages.html"><center>Restaurant Gallery</center></a>
    </div>

    </div>
	
</head>
</body>
</html>



