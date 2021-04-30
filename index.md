<!DOCTYPE html>
<html>
<head>
	<title>Home Page</title>
	<style type="text/css">
		*{
			box-sizing: border-box;
			font-family: 'Apercu Pro';
		}
		body{
			margin: 0;
			display: flex;
			flex-direction: row;
			flex-wrap: wrap;
			justify-content: space-around;
			background-color: #F4F6FA;
		}
		header, #top, #menu{
			text-align: center;
		}
		#title{
			text-align: left;
			font-size: 3.5em; 
			font-family: 'League Spartan';
		}
		#top, #menu{
			margin-bottom: 2em;
			border-radius: 15px;
			/*border: 0.2px solid black;*/
		}
		header, footer{
			width: 100%;
		}
		body, #top{
			align-items: center;
		}
		header{
			height: 10vh;
			background-color: #6ECBD9;
			margin-bottom: 1em;
			position: sticky;
			top: 0;
			z-index: 2;
		}
		#top{
			display: grid;
			/*position: relative;*/
			grid-template-columns: 1fr 2fr;
			width: 90%;
			height: 40vh;
			background-color: #BD8DC7;
			justify-items: center;
			overflow: hidden;
			align-items: center;
		}
		#top p{
			text-align: justify;
		}
		#top #toptext{
			width: 90%;
		}

		#menu{
			width: 30%;
			height: 80vh;
			background-color: #C1E679;
			display: flex;
			flex-direction: column;
			/*border: 1px solid black;*/
			align-items: center;
			/*justify-content: space-between;*/
			font-weight: bold;
			position: relative;
		}
		p{
			justify-self: left;
			font-size: 2em;
		}
		footer{
			color: black;
			height: 5vh;
			background-color: #F7EEC5;
			text-align: right;
		}
		#slide{
			width: 100%;
			height: 100%;
			overflow:hidden; 
			position:relative;
			display: flex;
			justify-content: space-around;
		}
		#slide img{
			position:absolute;
			align-self: center; 
			animation:slide 20s infinite;
			opacity:0;
			width: 45%;
			height: auto;
		}
		@keyframes slide {25%{opacity:1;} 40%{opacity:0;}}
 		#slide img:nth-child(4){animation-delay:0s;}
 		#slide img:nth-child(3){animation-delay:5s;}
 		#slide img:nth-child(2){animation-delay:10s;}
 		#slide img:nth-child(1){animation-delay:15s;}
		
		a:link, a:visited, a:hover, a:active{
			text-decoration: none;
			color: black;
		}

		a img{
			width: 75%;
		}
		.menutext{
			align-self: top;
			margin-top: 2vh;
			margin-bottom: 2vh; 
			font-size: 3em;
		}
		.menuimg{
			  display: block;
		}
		.text-wrapper{
			border-radius: 15px;
			position: absolute;
  			top: 0;
			bottom: 0;
			left: 0;
			right: 0;
			height: 100%;
			width: 100%;
			opacity: 0;
			transition: .5s ease;
			background-color: #B4D27ADD;
		}
		#menu:hover .text-wrapper{
			opacity: 1;
		}
		.ftext{
			color: white;
  			font-size: 20px;
  			position: absolute;
  			top: 50%;
  			left: 50%;
  			-webkit-transform: translate(-50%, -50%);
  			-ms-transform: translate(-50%, -50%);
  			transform: translate(-50%, -50%);
  			text-align: center;
		}


	</style>
</head>
<body>
	<header>
		<div id="title">E-CARDS ONLINE</div>
	</header>
	<div id="top">
		<div id="slide">
			<img src="images/sample.jfif">
			<img src="images/Wedding-Invitation-Cards.jpg">
			<img src="images/sample.jfif">
			<img src="images/Wedding-Invitation-Cards.jpg">
		</div>
		<div id="toptext">
			<p>Create your own e-invitation card</p>
		</div>
	</div>
	<a href="formal.html" id="menu">
		<div class="menutext menuimg">Formal</div>
		<img src="images/sample.jfif" class="menuimg">
		<div class="text-wrapper">
			<p class="ftext">For formal events like weddings, graduation ceremonies, etc.</p>
		</div>
	</a>
	<a href="informal.html" id="menu">
		<div class="menutext menuimg">Informal</div>
		<img src="images/sample.jfif" class="menuimg">
		<div class="text-wrapper" >
			<p class="ftext">For informal events like birthday parties, celebrations, etc.</p>
		</div>
	</a>
	<a href="" id="menu">
		<div class="menutext menuimg">Corporate</div>
		<img src="images/sample.jfif" class="menuimg">
		<div class="text-wrapper">
			<p class="ftext">For corperate events like expos, conferences, team-building events, etc.</p>
		</div>
	</a>
	<footer>Copyright</footer>

</body>
</html>