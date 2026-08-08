# Special-
Birthday wishes 
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width,
initial-scale=1.0">

<title>Birthday Surprise ❤️</title>


<style>

/* =====================================
   BASIC
===================================== */

*{
    box-sizing:border-box;
    -webkit-tap-highlight-color:transparent;
}

body{

    margin:0;

    min-height:100vh;

    overflow:hidden;

    font-family:
    Arial,
    sans-serif;

    background:
    linear-gradient(
        135deg,
        #ffb6d9,
        #ff5c9d,
        #d60050
    );

    color:white;

}


/* =====================================
   COMMON PAGE
===================================== */

.page{

    position:absolute;

    width:100%;
    height:100vh;

    display:none;

    justify-content:center;
    align-items:center;

    flex-direction:column;

    text-align:center;

    padding:20px;

}

.page.active{
    display:flex;
}


/* =====================================
   STARS
===================================== */

.star{

    position:fixed;

    color:white;

    font-size:22px;

    z-index:2;

    animation:
    starGlow 1.5s infinite alternate;

}

.star:nth-child(1){
    top:8%;
    left:8%;
}

.star:nth-child(2){
    top:18%;
    left:85%;
}

.star:nth-child(3){
    top:35%;
    left:12%;
}

.star:nth-child(4){
    top:45%;
    left:90%;
}

.star:nth-child(5){
    top:70%;
    left:7%;
}

.star:nth-child(6){
    top:78%;
    left:88%;
}

.star:nth-child(7){
    top:55%;
    left:50%;
}

@keyframes starGlow{

    from{
        opacity:.3;
        transform:scale(.8);
    }

    to{
        opacity:1;
        transform:scale(1.3);
    }

}


/* =====================================
   PAGE 1
===================================== */

#welcomePage{

    background:
    radial-gradient(
        circle,
        rgba(255,255,255,.25),
        transparent 50%
    );

}

.welcomeTitle{

    font-size:
    clamp(
        30px,
        8vw,
        60px
    );

    color:#fff;

    text-shadow:
    0 0 10px #ff004f,
    0 0 30px #ff004f,
    0 0 60px #ff004f;

    animation:
    titleGlow 2s infinite alternate;

}

@keyframes titleGlow{

    from{
        transform:scale(1);
    }

    to{
        transform:scale(1.05);
    }

}


.startButton{

    padding:
    17px 35px;

    border:none;

    border-radius:50px;

    background:
    linear-gradient(
        45deg,
        #8b0038,
        #ff0059
    );

    color:white;

    font-size:18px;

    font-weight:bold;

    box-shadow:
    0 0 15px #ff0059,
    0 0 40px #ff0059;

    cursor:pointer;

}


/* =====================================
   SHOOTING GAME
===================================== */

#gamePage{

    background:
    linear-gradient(
        #54206e,
        #c43b77 55%,
        #ff9dba
    );

}


/* Game title */

.gameTitle{

    position:absolute;

    top:15px;

    font-size:
    clamp(
        25px,
        7vw,
        45px
    );

    color:#fff;

    text-shadow:
    0 0 10px #000,
    0 0 25px #ff006a;

}


/* Score */

.scoreBox{

    position:absolute;

    top:70px;

    padding:
    8px 20px;

    border-radius:30px;

    background:
    rgba(0,0,0,.35);

    font-size:20px;

    font-weight:bold;

}


/* Game area */

.gameArea{

    position:relative;

    width:100%;

    max-width:600px;

    height:55vh;

    min-height:350px;

    overflow:hidden;

    border-radius:25px;

    background:

    linear-gradient(
        #442060,
        #8d346c 65%,
        #f0839f
    );

    border:
    2px solid
    rgba(255,255,255,.5);

    box-shadow:
    0 0 30px
    rgba(255,0,90,.5);

}


/* Moon */

.moon{

    position:absolute;

    top:30px;
    right:30px;

    width:65px;
    height:65px;

    border-radius:50%;

    background:#fff7c7;

    box-shadow:
    0 0 25px #fff;

}


/* Ground */

.ground{

    position:absolute;

    bottom:0;
    left:0;

    width:100%;
    height:70px;

    background:
    linear-gradient(
        #321537,
        #170b20
    );

}


/* Target Gate */

.target{

    position:absolute;

    right:30px;

    bottom:70px;

    width:120px;
    height:150px;

    border:
    10px solid #ffcc00;

    border-bottom:none;

    border-radius:
    70px 70px 0 0;

    background:
    rgba(255,0,60,.2);

    box-shadow:
    0 0 15px #ffd000,
    0 0 35px #ff5c00;

}


/* Target center */

.targetCenter{

    position:absolute;

    top:40px;
    left:25px;

    width:50px;
    height:50px;

    border-radius:50%;

    background:
    #ff1744;

    border:
    7px solid white;

    box-shadow:
    0 0 20px red;

}


/* Shooter */

.shooter{

    position:absolute;

    bottom:15px;
    left:40px;

    width:75px;
    height:55px;

    border-radius:
    20px 20px 10px 10px;

    background:
    linear-gradient(
        #ff4b86,
        #b40048
    );

    box-shadow:
    0 0 15px #ff0066;

}


/* Bow */

.bow{

    position:absolute;

    bottom:70px;
    left:60px;

    width:50px;
    height:80px;

    border:
    5px solid #ffd36b;

    border-left:none;

    border-radius:
    0 50% 50% 0;

    transform:
    rotate(-5deg);

}


/* Arrow */

.arrow{

    position:absolute;

    bottom:112px;
    left:75px;

    width:100px;
    height:5px;

    background:white;

    border-radius:10px;

    transform-origin:left center;

    transition:
    left .5s linear;

    box-shadow:
    0 0 8px white;

}


/* Arrow head */

.arrow:after{

    content:"";

    position:absolute;

    right:-10px;

    top:-6px;

    border-left:
    14px solid white;

    border-top:
    8px solid transparent;

    border-bottom:
    8px solid transparent;

}


/* Shoot button */

.shootButton{

    position:absolute;

    bottom:20px;

    right:20px;

    padding:
    13px 22px;

    border:none;

    border-radius:40px;

    background:
    #ff1744;

    color:white;

    font-size:17px;

    font-weight:bold;

    box-shadow:
    0 0 15px #ff1744;

}


/* Game instruction */

.gameInstruction{

    margin-top:15px;

    font-size:16px;

}


/* =====================================
   GAME COMPLETE
===================================== */

#gameComplete{

    display:none;

    position:absolute;

    inset:0;

    background:
    rgba(40,0,30,.88);

    z-index:100;

    justify-content:center;
    align-items:center;

    flex-direction:column;

}


#gameComplete h1{

    font-size:
    clamp(
        35px,
        9vw,
        60px
    );

    color:#ffe600;

    text-shadow:
    0 0 15px #ff9d00,
    0 0 40px #ff1744;

}


.continueButton{

    padding:
    15px 28px;

    border:none;

    border-radius:40px;

    background:
    linear-gradient(
        45deg,
        #ff004f,
        #ff7ab0
    );

    color:white;

    font-size:18px;

    font-weight:bold;

}


/* =====================================
   PUZZLE
===================================== */

#puzzlePage{

    background:
    linear-gradient(
        135deg,
        #ff8fbd,
        #d90055
    );

}


.puzzleCard{

    width:
    min(92%,430px);

    padding:35px 25px;

    border-radius:30px;

    background:
    rgba(255,255,255,.18);

    backdrop-filter:
    blur(15px);

    border:
    2px solid
    rgba(255,255,255,.5);

    box-shadow:
    0 0 40px
    rgba(80,0,50,.5);

}


.puzzleCard h2{

    font-size:30px;

}


.puzzleButton{

    padding:
    15px 25px;

    border:none;

    border-radius:40px;

    background:#8b0038;

    color:white;

    font-size:17px;

    font-weight:bold;

}


/* =====================================
   CAKE PAGE
===================================== */

#cakePage{

    background:
    linear-gradient(
        135deg,
        #ff9ac5,
        #ed2868,
        #a80042
    );

}


.cakeTitle{

    font-size:
    clamp(
        32px,
        8vw,
        55px
    );

    color:#fffde7;

    text-shadow:
    0 0 8px #7a0038,
    0 0 20px #ff004f;

}


.instruction{

    font-size:17px;

}


/* Cake */

.cake{

    position:relative;

    width:300px;
    height:200px;

    margin-top:30px;

}


/* Candles */

.candles{

    position:absolute;

    top:-70px;
    left:25px;

    width:250px;

    display:flex;

    justify-content:
    space-around;

}


.candle{

    position:relative;

    width:20px;
    height:65px;

    background:
    repeating-linear-gradient(
        45deg,
        #ff1744 0px,
        #ff1744 8px,
        white 8px,
        white 16px
    );

    border-radius:5px;

    cursor:pointer;

}


/* Flame */

.flame{

    position:absolute;

    top:-34px;
    left:-5px;

    font-size:27px;

    animation:
    flameMove .4s infinite alternate;

}


@keyframes flameMove{

    from{
        transform:
        scale(1)
        rotate(-5deg);
    }

    to{
        transform:
        scale(1.2)
        rotate(5deg);
    }

}


.candle.off .flame{
    display:none;
}


/* Cake cream */

.cream{

    position:absolute;

    bottom:100px;
    left:15px;

    width:270px;
    height:50px;

    background:
    #fff;

    border-radius:
    25px 25px 10px 10px;

    box-shadow:
    0 0 20px white;

}


/* Cake body */

.cakeBody{

    position:absolute;

    bottom:35px;
    left:20px;

    width:260px;
    height:80px;

    background:
    linear-gradient(
        #ff1744,
        #b8003c
    );

    border-radius:
    10px 10px 20px 20px;

}


/* Plate */

.plate{

    position:absolute;

    bottom:15px;

    width:300px;
    height:25px;

    background:white;

    border-radius:50%;

}


/* =====================================
   BIRTHDAY MESSAGE
===================================== */

#birthdayMessage{

    display:none;

    position:absolute;

    inset:0;

    z-index:200;

    background:
    rgba(75,0,35,.82);

    justify-content:center;
    align-items:center;

    flex-direction:column;

    padding:20px;

}


/* Birthday title */

#birthdayMessage h1{

    font-size:
    clamp(
        42px,
        11vw,
        90px
    );

    margin:10px;

    color:#ffe600;

    font-weight:900;

    text-shadow:
    0 0 5px #8b0038,
    0 0 15px #ff1744,
    0 0 35px #ff8a00,
    3px 3px 0 #8b0038;

    animation:
    birthdayGlow 1s infinite alternate;

}


@keyframes birthdayGlow{

    from{
        transform:scale(1);
    }

    to{
        transform:scale(1.06);
    }

}


#birthdayMessage h2{

    color:#ffffff;

    font-size:
    clamp(
        20px,
        5vw,
        32px
    );

    text-shadow:
    0 0 10px #ff0055;

}


#birthdayMessage p{

    color:#fff;

    font-size:18px;

    line-height:1.7;

    max-width:500px;

    text-shadow:
    0 2px 5px #6b0030;

}


/* =====================================
   BIRTHDAY IMAGES
===================================== */

.birthdayPhotos{

    display:flex;

    gap:15px;

    justify-content:center;

    margin-top:10px;

}


.birthdayPhotos img{

    width:90px;
    height:90px;

    object-fit:cover;

    border-radius:20px;

    border:
    3px solid white;

    box-shadow:
    0 0 15px #ff0055;

}


/* =====================================
   BALLOONS
===================================== */

.balloon{

    position:fixed;

    bottom:-100px;

    font-size:50px;

    z-index:300;

    animation:
    balloonFly 5s linear forwards;

}


@keyframes balloonFly{

    from{

        transform:
        translateY(0)
        rotate(-5deg);

    }

    to{

        transform:
        translateY(-120vh)
        rotate(15deg);

        opacity:0;

    }

}


/* =====================================
   CONFETTI
===================================== */

.confetti{

    font-size:35px;

    margin-bottom:10px;

}


/* =====================================
   MOBILE
===================================== */

@media(max-width:600px){

    .gameArea{

        height:52vh;

        min-height:330px;

    }


    .target{

        right:15px;

        transform:
        scale(.85);

    }


    .shootButton{

        bottom:15px;

        right:15px;

    }


    .birthdayPhotos img{

        width:75px;
        height:75px;

    }


    .cake{

        transform:
        scale(.85);

    }

}

</style>

</head>


<body>


<!-- =====================================
     STARS
===================================== -->

<span class="star">⭐</span>
<span class="star">✨</span>
<span class="star">⭐</span>
<span class="star">✨</span>
<span class="star">⭐</span>
<span class="star">✨</span>
<span class="star">⭐</span>



<!-- =====================================
     MUSIC
===================================== -->

<audio
id="music"
loop>

<source
src="birthday.mp3"
type="audio/mpeg">

</audio>



<!-- =====================================
     PAGE 1
===================================== -->

<section
id="welcomePage"
class="page active">


<h1 class="welcomeTitle">

🎁 A Little Surprise For You ❤️

</h1>


<p>

But first...<br>

🎮 Complete a little game!

</p>


<button
class="startButton"
onclick="startGame()">

🎮 START GAME

</button>


</section>



<!-- =====================================
     GAME PAGE
===================================== -->

<section
id="gamePage"
class="page">


<h1 class="gameTitle">

🏹 HIT THE TARGET 🎯

</h1>


<div class="scoreBox">

Score:
<span id="score">0</span>
/
3

</div>



<div class="gameArea">


<div class="moon"></div>


<!-- Target -->

<div
class="target"
id="target">

<div
class="targetCenter">

</div>

</div>


<!-- Shooter -->

<div class="shooter"></div>


<div class="bow"></div>


<div
class="arrow"
id="arrow">

</div>


<div class="ground"></div>


<button
class="shootButton"
onclick="shootArrow()">

🏹 SHOOT

</button>


</div>


<p class="gameInstruction">

🎯 Hit the red center 3 times to unlock the birthday surprise!

</p>



<!-- GAME COMPLETE -->

<div id="gameComplete">


<h1>

🎉 YOU DID IT! 🎉

</h1>


<p>

The birthday surprise is unlocked! ❤️

</p>


<button
class="continueButton"
onclick="goPuzzle()">

🎁 CONTINUE

</button>


</div>


</section>



<!-- =====================================
     PUZZLE PAGE
===================================== -->

<section
id="puzzlePage"
class="page">


<div class="puzzleCard">


<h2>

💖 One More Little Surprise 💖

</h2>


<p>

You completed the game! 🎉<br><br>

Now open the birthday surprise... 🎁

</p>


<button
class="puzzleButton"
onclick="goCake()">

✨ OPEN SURPRISE ✨

</button>


</div>


</section>



<!-- =====================================
     CAKE PAGE
===================================== -->

<section
id="cakePage"
class="page">


<h1 class="cakeTitle">

🎂 MAKE A WISH! 🎂

</h1>


<p class="instruction">

Tap all the candles to blow them out 🕯️

</p>



<div class="cake">


<!-- Candles -->

<div class="candles">


<div
class="candle"
onclick="blowCandle(this)">

<div class="flame">
🔥
</div>

</div>


<div
class="candle"
onclick="blowCandle(this)">

<div class="flame">
🔥
</div>

</div>


<div
class="candle"
onclick="blowCandle(this)">

<div class="flame">
🔥
</div>

</div>


<div
class="candle"
onclick="blowCandle(this)">

<div class="flame">
🔥
</div>

</div>


<div
class="candle"
onclick="blowCandle(this)">

<div class="flame">
🔥
</div>

</div>


</div>


<div class="cream"></div>


<div class="cakeBody"></div>


<div class="plate"></div>


</div>



<!-- =====================================
     FINAL MESSAGE
===================================== -->

<div id="birthdayMessage">


<div class="confetti">

🎉 🎊 ✨ 🎈 ✨ 🎊 🎉

</div>


<h1>

HAPPY BIRTHDAY ❤️

</h1>


<h2>

🎂 Wishing You A Beautiful Day 🎂

</h2>


<!-- PUBLIC IMAGES -->

<div class="birthdayPhotos">


<img
src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=300&q=80"
alt="Birthday Cake"
onerror="this.style.display='none';">


<img
src="https://images.unsplash.com/photo-1513159446162-54eb8bdaa79b?auto=format&fit=crop&w=300&q=80"
alt="Birthday Balloons"
onerror="this.style.display='none';">


</div>


<p>

May your life always be filled with<br>

happiness, smiles, love and beautiful memories! 💖

</p>


<div class="confetti">

❤️ 💕 ❤️ 💕 ❤️

</div>


</div>


</section>



<script>

/* =====================================
   VARIABLES
===================================== */

let score = 0;

let candlesLeft = 5;



/* =====================================
   CHANGE PAGE
===================================== */

function showPage(id){

    document
    .querySelectorAll(".page")
    .forEach(function(page){

        page.classList.remove("active");

    });


    document
    .getElementById(id)
    .classList.add("active");

}



/* =====================================
   START GAME
===================================== */

function startGame(){

    showPage("gamePage");


    let music =
    document.getElementById("music");


    music.play().catch(function(){

        console.log(
        "Music needs user interaction.");

    });

}



/* =====================================
   SHOOT ARROW
===================================== */

function shootArrow(){

    let arrow =
    document.getElementById("arrow");


    /* Arrow animation */

    arrow.style.left="75px";


    setTimeout(function(){

        arrow.style.left="calc(100% - 150px)";


    },50);


    setTimeout(function(){

        score++;

        document
        .getElementById("score")
        .innerText=score;


        /* Reset arrow */

        arrow.style.left="75px";


        if(score>=3){

            document
            .getElementById("gameComplete")
            .style.display="flex";

        }

    },550);

}



/* =====================================
   PUZZLE
===================================== */

function goPuzzle(){

    showPage("puzzlePage");

}



/* =====================================
   CAKE
===================================== */

function goCake(){

    showPage("cakePage");

}



/* =====================================
   CANDLE
===================================== */

function blowCandle(candle){

    if(
        candle.classList
        .contains("off")
    ){

        return;

    }


    candle.classList.add("off");


    candlesLeft--;


    if(candlesLeft===0){

        setTimeout(function(){

            document
            .getElementById("birthdayMessage")
            .style.display="flex";


            createBalloons();


        },700);

    }

}



/* =====================================
   BALLOONS
===================================== */

function createBalloons(){

    let balloonList=[
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈",
        "🎈"
    ];


    balloonList.forEach(function(){

        let balloon =
        document.createElement("div");


        balloon.className=
        "balloon";


        balloon.innerHTML=
        "🎈";


        balloon.style.left=
        Math.random()*100+"%";


        balloon.style.animationDelay=
        Math.random()*2+"s";


        document.body.appendChild(
        balloon);

    });

}

</script>


</body>

</html>
