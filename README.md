<!DOCTYPE html>
<html>
<head>

	<link rel="stylesheet" href="css/jquery.mobile.icons.min.css" />
	<link rel="stylesheet" href="css/Design.min.css" />
	<link rel="stylesheet" href="css/jquery.mobile.structure-1.4.5.min.css" />
<style>
  body
  	{
  	margin:0;
  	}
  
  <!--==========================For image animations======================-->
  @-webkit-keyframes out
  	{
  		0% {top:30px;}
  		30% {top:60px;}
  		50% {transform:rotate(-80deg) scale(0.8,0.8);}
  		100% {top:-1000px;transform:rotate(-5000)}
  	}
  
  @keyframes out
  	{
  		0% {top:30px;}
  		30% {top:60px;}
  		50% {transform:rotate(-80deg) scale(0.8,0.8);}
  		100% {top:-1000px;transform:rotate(-5000)}
  	}
  
  	@-webkit-keyframes out2
  	{
  		0% {top:30%;}
  		30% {transform:rotate(-80deg) scale(0.8,0.8);}
  		100% {top:-1000px;transform:rotate(-5000deg)}
  	}
  		@keyframes out2
  	{
  		0% {top:30%;}
  		30% {transform:rotate(-80deg) scale(0.8,0.8);}
  		100% {top:-1000px;transform:rotate(-5000deg)}
  	}
  @-webkit-keyframes in
  	{
  		0% {top:-1000px;transform:rotate(-5000)}
  		30% {transform:rotate(-80deg) scale(0.1,0.1);}
  		50% {top:60px;}
  		100% {top:30%;transform:rotate(0deg) scale(1,1);}
  	}
  @keyframes in
  	{
  		0% {top:-1000px;transform:rotate(-5000)}
  		30% {transform:rotate(-80deg) scale(0.5,0.5);}
  		50% {top:60px;}
  		100% {top:30%;transform:rotate(0deg) scale(1,1);}
  	}
  @-webkit-keyframes shuffle1
  	{
  	0% {left:0px;}
  	10% {left:300px}
  	20% {left:-150px}
  	30% {left:150px}
  	40% {left:-150px}
  	50% {left:150px}
  	60% {left:-150px}
  	70% {left:150px}
  	80% {left:-150px}
  	90% {left:150px}
  	100% {left:0px}
  	}
  @keyframes shuffle1
  	{
  	0% {left:0px;}
  	10% {left:300px}
  	20% {left:-150px}
  	30% {left:150px}
  	40% {left:-150px}
  	50% {left:150px}
  	60% {left:-150px}
  	70% {left:150px}
  	80% {left:-150px}
  	90% {left:150px}
  	100% {left:0px}
  	}
  
  @-webkit-keyframes shuffle2
  	{
  	0% {right:0px;}
  	10% {right:300px;}
  	20% {right:-150px;}
  	30% {right:150px;}
  	40% {right:-150px;}
  	50% {right:150px;}
  	60% {right:-150px;}
  	70% {right:150px;}
  	80% {right:-150px;}
  	90% {right:150px;}
  	100% {right:0px;}
  	}
  @keyframes shuffle2
  	{
  	0% {right:0px;}
  	10% {right:300px;}
  	20% {right:-150px;}
  	30% {right:150px;}
  	40% {right:-150px;}
  	50% {right:150px;}
  	60% {right:-150px;}
  	70% {right:150px;}
  	80% {right:-150px;}
  	90% {right:150px;}
  	100% {right:0px;}
  	}
  @-webkit-keyframes arrows
  	{
  	from {transform:scale(1.1,1.1) rotate(10deg);}
  	to {transform:scale(1,1) rotate(0deg);}
  	}
  @keyframes arrows
  	{
  	from {transform:scale(1.1,1.1) rotate(10deg);}
  	to {transform:scale(1,1) rotate(0deg);}
  	}
  @-webkit-keyframes arrow
  	{
  	from {transform:scale(1,1)}
  	to {transform:scale(0.9,0.9)}
  	}
  @keyframes arrow
  	{
  	from {transform:scale(1,1)}
  	to {transform:scale(0.9,0.9)}
  	}
  @-webkit-keyframes banner
  	{
  	from {transform:scale(0.9,0.9)}
  	to {transform:scale(1,1)}
  	}
  @keyframes banner
  	{
  	from {transform:scale(0.9,0.9)}
  	to {transform:scale(1,1)}
  	}
  @-webkit-keyframes bannerwave
  	{
  	from {top:0px;)}
  	to {top:20px;}
  	}
  @keyframes bannerwave
  	{
  	from {top:0px;)}
  	to {top:20px;}
  	}
  	
  	<!--==========================assigning animations and styles per class and id======================-->
  #try
  	{
  	-webkit-animation:arrows 0.3s;
  	animation:arrows 0.3s;
  	}
  .ar
  	{
  	-webkit-animation:arrow 1s alternate infinite;
  	 animation:arrow 1s alternate infinite;
  	}
  h1,h2
  	{
  	color:white;
  	}
  .color
  	{
  	background-color:#694b28;
  	}
  #game
  	{
  	background-color:rgba(249, 249, 249, 0);
  	}
  img 
  	{
  		margin-left:auto;
  		margin-right:auto;
  		width:100%;
  	}
  .back
  	{
  		width:100%;
  		position:fixed;
  		z-index:-1;
  	}
  .first
  	{
  		margin-left:auto;
  		margin-right:auto;
  		-webkit-animation:banner 0.3s;
  		animation:banner 0.3s;
  		width:100%;
  		position:absolute;
  		z-index:3;
  		top:30px;
  	}
  .second
  	{
  
  		width:100%;
  		position:fixed;
  		z-index:2;
  	}
  .datas
  	{
  		width:100%;
  		position:absolute;
  		z-index:1;
  	}
  .cupleft
  	{
  	position:relative;
  	-webkit-animation: shuffle1 1s;
  	 animation: shuffle1 1s;
  	}
  .cupright
  	{
  	position:relative;
  	-webkit-animation: shuffle2 0.7s;
  	 animation: shuffle2 0.7s;
  	}
  .cupmid
  	{
  	position:relative;
  	-webkit-animation: shuffle1 0.4s;
  	 animation: shuffle1 0.4s;
  	}
  .fbframe
  	{
  	align:center;
  	margin-left:auto;
  	margin-right:auto;
  	width:5em;
  	}
  .fbpapels
  	{
  	top:-1000px;
  	position:absolute;
  	}

</style>
<script src="js/jquery-1.11.1.min.js"></script>
<script src="js/cordova-1.5.js"></script>
<script src="js/jquery.mobile-1.4.5.min.js"></script>
<script>
//Declarations of variables to be use
var control=1;
var inputguess=0;
var trys=10;
var score=0;
document.getElementById('score').innerHTML=score;

function life(){
	var lifes=document.getElementById('life');
	switch(trys)
	{
	//Life meter
		case 1:
			lifes.setAttribute("src","images/hearts/1.png"); break;
		case 2:
			lifes.setAttribute("src","images/hearts/2.png"); break;
		case 3:
			lifes.setAttribute("src","images/hearts/3.png"); break;
		case 4:
			lifes.setAttribute("src","images/hearts/4.png"); break;
		case 5:
			lifes.setAttribute("src","images/hearts/5.png"); break;
		case 6:
			lifes.setAttribute("src","images/hearts/6.png"); break;
		case 7:
			lifes.setAttribute("src","images/hearts/7.png"); break;
		case 8:
			lifes.setAttribute("src","images/hearts/8.png"); break;
		case 9:
			lifes.setAttribute("src","images/hearts/9.png"); break;
		case 10:
			lifes.setAttribute("src","images/hearts/10.png"); break;
		
	}

}

//This functions are from images that has been guessed. Guess number
function guesss1()
{
	if(control==1)
	{
	control=0;
	inputguess=0;
	chck();
	}
}
function guesss2()
{
	if(control==1)
	{
	control=0;
	inputguess=1;
	chck();
	}
}
function guesss3()
{
	if(control==1)
	{
	control=0;
	inputguess=2;
	chck();
	}
}
// functions in setting a ball in random position
function cup1()
	{
			var image1=document.getElementById('guess1');
			var image2=document.getElementById('guess2');
			var image3=document.getElementById('guess3');
				image1.setAttribute("src","images/open.png");
				image2.setAttribute("src","images/none.png");
				image3.setAttribute("src","images/none.png");
	}
function cup2()
	{
			var image1=document.getElementById('guess1');
			var image2=document.getElementById('guess2');
			var image3=document.getElementById('guess3');
				image1.setAttribute("src","images/none.png");
				image2.setAttribute("src","images/open.png");
				image3.setAttribute("src","images/none.png");
				
	}
function cup3()
	{
			var image1=document.getElementById('guess1');
			var image2=document.getElementById('guess2');
			var image3=document.getElementById('guess3');
				image1.setAttribute("src","images/none.png");
				image2.setAttribute("src","images/none.png");
				image3.setAttribute("src","images/open.png");
	
	}
	//function in checking whether the guess and the randNum is equal or not. This sets also whether the score of the player was the high score. It sets it in local storage
function chck(){
	var randNum = Math.floor(Math.random()*3);
	if(randNum==0)
		{
		cup1();
		}
	else if(randNum==1)
		{
		cup2();	
		}
	else if(randNum==2)
		{
		cup3();
		}

	if(inputguess==randNum)
	{
	
	
		document.getElementById('stats').setAttribute("src","images/correct.png");
		score=score+1;
		document.getElementById('score').innerHTML=score;
		if(trys<10)
		{
		trys=trys+1;
		}
		

	}	
	else {
		trys=trys-1;
		

		document.getElementById('stats').setAttribute("src","images/wrong.png");
	}
		

		

	var highs=localStorage.getItem("highscore");
	if(score>highs){localStorage.setItem("highscore",score);}
		$("#try").show();
		$(".ar").hide();
		document.getElementById('highs').innerHTML = "High Score: " + highs;
		
		if(trys==0)
		{
		var res=confirm("Total score : " + score + ". Restart the game?");
			if(res==true)
				{
				trys=10;
				score=0;
				document.getElementById('score').innerHTML=score;
				$("#try").hide();
				$(".ar").show();
				again();
				}
			else
			{
				
		
				bannerin();
			}
		}
		life();
}

// This function occurs when user taps the retry button. it refreshes every cup to be close. It will animate images also
function again()
{
		control=1;
			var image1=document.getElementById('guess1');
			var image2=document.getElementById('guess2');
			var image3=document.getElementById('guess3');

		
			$("#try").hide(2,function(){
				image1.setAttribute("style","-webkit-animation: shuffle2 1s;animation: shuffle2 1s;");
				image2.setAttribute("style","-webkit-animation: shuffle2 0.6s;animation: shuffle2 0.6s;");
				image3.setAttribute("style","-webkit-animation: shuffle2 0.8s;animation: shuffle2 0.8s;");
				
				$(".ar").show(0,function(){
				image1.setAttribute("src","images/close.png");
				image2.setAttribute("src","images/close.png");
				image3.setAttribute("src","images/close.png");
			});
			document.getElementById('stats').setAttribute("src","images/play.png");
			});
		

				

}

//this function occurs when the Guess Where banner in start of the app was clicked.
function bannerout()
	{
		document.getElementById('banner').setAttribute("style","-webkit-animation:out 1.1s;animation: out 1.1s;");
		$("#blur").hide();
		var myInterval=setInterval(function(){
		$("#banner").hide();
				trys=10;
				score=0;
				$("#try").hide();
				$(".ar").show();


			control=1;
			clearInterval(myInterval);
		},500);
		
	}
//When the game ends and the user dont want to restart, this will occur. It gets back the App banner 
function bannerin()
	{	
		
		$("#blur").show();
		document.getElementById('banner').setAttribute("style","-webkit-animation:in 0.5s;animation:in 0.5s");
		$("#banner").show();
		
	}
	//this is for the fb button. It sets the image in another image.
function fblight()
	{
		document.getElementById('fbbutton').setAttribute("src","images/fbbuttonhover.png");

	}
	//this occurs when the fb share and like banner was closed. It set the fb button to its normal interface
function fbdark()
	{
		document.getElementById('fbbutton').setAttribute("src","images/fbbutton.png");		
		$("#blur").show();
		$("#papel").show();
		document.getElementById('papel').setAttribute("style","-webkit-animation:in 0.5s;animation:in 0.5s;top:30%");
	}
	//this is for the close button of fb share and like banner. It sets the image in another image.
function closea()
	{
		document.getElementById('closebut').setAttribute("src","images/closebuttonlight.png");
		
	}
	//this occurs when the fb share and like banner was open. It set the close button of fb share and like banner to its normal interface
function closea2()
	{	
		$("#blur").hide();
		document.getElementById('papel').setAttribute("style","-webkit-animation:out2 1.1s;animation: out2 1.1s;");
			var myIntervals=setInterval(function(){
		$("#papel").hide();
		

			clearInterval(myIntervals);
		},500);
		
	
		document.getElementById('closebut').setAttribute("src","images/closebutton.png");

	}

</script>
<script id="tinyhippos-injected">if (window.top.ripple) { window.top.ripple("bootstrap").inject(window, document); }</script><head><meta http-equiv="Content-Type" content="text/html; charset=windows-1252">

</head>

<body>
<!--==============================The div of the whole page================================-->
	<div id="game" data-role="page">
		<div class="color" data-role="main">
		<!--==============================The div of the contents of the page================================-->
			<div data-role="content" style="margin:0;padding:0">
			
			<img class="back" src="images/back.png">
			
			
				<div class="datas" style="margin-left:auto;margin-right:auto">
					<div align="center" class="ui-grid-b" > 
						<div class="ui-block-a">
							<!--==============================Image of the life meter================================-->
							<img id="life" src="images/hearts/10.png"  >
					
						</div>
						<div class="ui-block-b">
						<!--==============================Image of the Guess status, Correct or Wrong or Play================================-->
							<img id="stats" src="images/play.png"  >
						</div>
						<div class="ui-block-c">
							<br>
							<div style="z-index:-1;position:absolute;">
							<!--==============================Image of the background of the score ================================-->
								<img id="life" src="images/kahoy.png" style="width:70%">
							</div>
							<div style="color:white;z-index:-1;position:relative;width:100%;">
							<!--==============================Score display================================-->
								<p style="top:-15px;position:relative">Score</p>
								<h3 id="score" style="top:-33px;position:relative">0</h3>
							</div>
						</div>
					</div>
					<!--==============================Cups and Arrow Images. Placed in a ui-grid-b of jquery mobile================================-->
				<div align="center" class="ui-grid-b" > 
					<div class="ui-block-a">
						<img id="guess1" onclick="guesss1()" src="images/close.png" class="cupleft">
						<img class="ar"  src="images/arrow.png">
					</div>
					<div class="ui-block-b" style="margin:0">
						<img id="guess2" onclick="guesss2()" src="images/close.png" class="cupmid" >
						<img class="ar"  src="images/arrow.png">
					</div>
					<div class="ui-block-c">
						<img id="guess3" onclick="guesss3()" src="images/close.png" class="cupright">
						<img class="ar"  src="images/arrow.png">
					</div>
				</div>
				<div align="center" class="ui-grid-b" > 
					<div class="ui-block-a">
				
					</div>
					<div class="ui-block-b">
					<!--==============================Image of the retry button================================-->
						<img id="try" onclick="again()" src="images/retry.png">
					</div>
					<div class="ui-block-c">
					
					</div>
				</div>
				<div align="center"style="z-index:-1;position:absolute;width:100%">
				<!--==============================Image of the background of hight score and fb button================================-->
					<img style="width:70%;" src="images/box.png">
				</div>
					<div style="z-index:1;position:relative;margin-left:auto;margin-right:auto;">
						
						<div  align="center"id="fbframe" style="margin-left:auto;margin-right:auto">
						<!--==============================high score and fb button image================================-->
							<h1 align="center" id="highs"></h1>
							
							<img id="fbbutton" onmousedown="fblight()" onmouseup="fbdark()" style="width:40%" src="images/fbbutton.png">
									
						</div>		
							
					</div>		
		
				</div>
			</div>
		</div>
	</div>
	
<!--==============================div for share and like banner. named fbpapel cause it looks like a paper.================================-->
	<div class="first fbpapel" id="papel" align="center">
		<div style="z-index:-1;position:absolute;">
			<img  style="width:80%;position:relative;z-index:1" src="images/fbpapel.png">
		</div>
		<div style="color:white;z-index:-1;position:relative;width:100%;">
				<h2 style="top:10px;" >Share and Like Us</h2>

			<iframe src="http://www.facebook.com/plugins/like.php?href=http%3A%2F%2Ffacebook.com/GuessWhere30&amp;
			width=500&amp;layout=standard&amp;action=like&amp;show_faces=false&amp;share=true&amp;height=15"
			height="50"
			scrolling="no"
	     frameborder="0"
	     allowTransparency="true">
			</iframe>
																	
		</div>
		<br>
			<img id="closebut" onmousedown="closea()" onmouseup="closea2()" style="width:25%;position:relative;z-index:1" src="images/closebutton.png">
				
		</div>
									
	<div align="center" id="blur" class="second">
		<img src="images/blur.png">
	</div>
									
	<div id="banner" class="first" onclick="bannerout()">
								
		<img class="center" src="images/first.png">
	</div>
	
<script>
var highs=localStorage.getItem("highscore");
document.getElementById('highs').innerHTML = "High Score: " + highs;
$("#try").hide();
//cups button script
	$("#try").click(function(){
				$("img#guess1").css({"-webkit-animation":"shuffle1 0.3s","animation":"shuffle1 0.3s"});
				$("img#guess2").css({"-webkit-animation":"shuffle2 0.3s","animation":"shuffle1 0.3s"});
				$("img#guess3").css({"-webkit-animation":"shuffle2 0.3s","animation":"shuffle1 0.3s"});
document.getElementById('score').innerHTML=score;
});

	$("#papel").hide();

</script>						
</body>

</html>
