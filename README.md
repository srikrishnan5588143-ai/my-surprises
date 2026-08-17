# my-surprises
photo1.jpg
photo2.jpg
photo3.jpg
photo4.jpg
photo5.jpg
surprise.<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<meta name="theme-color" content="#ff4f87">

<title>10 Little Surprises ❤️</title>

<style>

/* =========================
   BASIC
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    Arial,
    sans-serif;

    background:#ffe8f0;
    color:#542b3a;

    overflow-x:hidden;
}

button,
input,
textarea{
    font-family:inherit;
}

button{
    cursor:pointer;
    border:none;
}

/* =========================
   LOGIN
========================= */

#loginPage{

    min-height:100vh;

    display:flex;

    align-items:center;

    justify-content:center;

    padding:20px;

    background:
    radial-gradient(
        circle at top left,
        #ffffff,
        transparent 35%
    ),

    linear-gradient(
        135deg,
        #ffd1e1,
        #fff5f8
    );
}

.loginCard{

    width:100%;

    max-width:420px;

    background:white;

    padding:35px 25px;

    border-radius:30px;

    text-align:center;

    box-shadow:
    0 20px 60px
    rgba(220,40,100,.18);
}

.loginTeddy{

    font-size:100px;

    animation:
    teddyBounce 2s infinite;
}

.loginCard h1{

    margin:15px 0 8px;

    color:#ed3572;

    font-size:30px;
}

.loginCard p{

    color:#777;

    line-height:1.6;

    margin-bottom:22px;
}

#nameInput{

    width:100%;

    padding:16px;

    border:2px solid #ffd0df;

    border-radius:16px;

    outline:none;

    text-align:center;

    font-size:16px;

    margin-bottom:12px;
}

.startButton{

    width:100%;

    padding:16px;

    border-radius:16px;

    color:white;

    font-size:16px;

    font-weight:bold;

    background:
    linear-gradient(
        135deg,
        #f53172,
        #ff88ac
    );

    box-shadow:
    0 10px 25px
    rgba(240,40,100,.25);
}

/* =========================
   APP
========================= */

#app{

    display:none;

    min-height:100vh;
}

/* =========================
   EDIT BUTTON
========================= */

.editButton{

    position:fixed;

    right:15px;

    top:15px;

    z-index:1000;

    padding:10px 15px;

    border-radius:20px;

    background:white;

    color:#e83470;

    font-weight:bold;

    box-shadow:
    0 5px 20px
    rgba(0,0,0,.15);
}

/* =========================
   PAGES
========================= */

.page{

    display:none;

    min-height:100vh;

    min-height:100svh;

    padding:
    90px 20px 50px;

    position:relative;

    text-align:center;

    align-items:center;

    justify-content:center;

    overflow:hidden;
}

.page.active{

    display:flex;
}

.content{

    width:100%;

    max-width:450px;

    position:relative;

    z-index:10;
}

.pageNumber{

    position:absolute;

    top:18px;

    left:18px;

    padding:8px 14px;

    background:white;

    color:#e73570;

    border-radius:20px;

    font-size:13px;

    font-weight:bold;
}

.title{

    color:#e93671;

    font-size:
    clamp(27px,7vw,38px);

    line-height:1.2;

    margin-bottom:18px;
}

.message{

    font-size:
    clamp(16px,4.5vw,19px);

    line-height:1.7;

    margin:18px auto;
}

.teddy{

    font-size:
    clamp(80px,28vw,125px);

    margin:15px;

    animation:
    teddyBounce 2s infinite;
}

@keyframes teddyBounce{

    0%,100%{
        transform:translateY(0);
    }

    50%{
        transform:translateY(-15px);
    }
}

/* =========================
   SPEECH
========================= */

.speech{

    background:white;

    padding:20px;

    max-width:350px;

    margin:20px auto;

    border-radius:25px;

    color:#df326c;

    font-weight:bold;

    line-height:1.6;

    box-shadow:
    0 10px 35px
    rgba(210,40,100,.15);
}

/* =========================
   BUTTONS
========================= */

.voiceButton{

    padding:11px 18px;

    border-radius:22px;

    background:white;

    color:#e73570;

    font-weight:bold;

    box-shadow:
    0 5px 15px
    rgba(0,0,0,.10);
}

.nextButton{

    margin-top:18px;

    padding:15px 27px;

    border-radius:28px;

    background:
    linear-gradient(
        135deg,
        #f33370,
        #ff83a7
    );

    color:white;

    font-weight:bold;

    box-shadow:
    0 10px 25px
    rgba(240,40,100,.25);
}

/* =========================
   PHOTO
========================= */

.photoFrame{

    background:white;

    padding:9px;

    border-radius:25px;

    max-width:380px;

    margin:20px auto;

    box-shadow:
    0 15px 40px
    rgba(200,40,100,.18);
}

.photoFrame img{

    display:block;

    width:100%;

    height:420px;

    object-fit:cover;

    border-radius:18px;
}

/* =========================
   VIDEO
========================= */

.videoFrame{

    max-width:380px;

    margin:20px auto;

    background:#111;

    padding:7px;

    border-radius:25px;
}

.videoFrame video{

    width:100%;

    max-height:450px;

    display:block;

    border-radius:18px;
}

/* =========================
   GIFT
========================= */

.gift{

    font-size:
    clamp(90px,30vw,140px);

    margin:20px;

    animation:
    giftAnimation 1.4s infinite;
}

@keyframes giftAnimation{

    0%,100%{
        transform:scale(1) rotate(0);
    }

    50%{
        transform:scale(1.12) rotate(6deg);
    }
}

.giftMessage{

    display:none;

    padding:20px;

    background:white;

    border-radius:22px;

    color:#df326c;

    font-weight:bold;

    line-height:1.6;
}

/* =========================
   MEMORY GRID
========================= */

.memoryGrid{

    display:grid;

    grid-template-columns:
    repeat(2,1fr);

    gap:10px;

    max-width:380px;

    margin:20px auto;
}

.memoryGrid img{

    width:100%;

    height:180px;

    object-fit:cover;

    border-radius:18px;
}

/* =========================
   HEART ANIMATION
========================= */

.heart{

    position:fixed;

    bottom:-50px;

    pointer-events:none;

    z-index:2;

    animation:
    heartAnimation
    linear forwards;
}

@keyframes heartAnimation{

    0%{

        transform:
        translateY(0)
        rotate(0)
        scale(.7);

        opacity:0;
    }

    15%{
        opacity:1;
    }

    100%{

        transform:
        translateY(-115vh)
        rotate(360deg)
        scale(1.3);

        opacity:0;
    }
}

/* =========================
   FINAL PAGE
========================= */

.finalPage{

    color:white;

    background:
    radial-gradient(
        circle at top,
        #ffb1c9,
        #ff427a 60%,
        #b81250
    );
}

.finalPage .title{

    color:white;
}

.finalPage .message{

    color:white;
}

.finalTeddy{

    font-size:
    clamp(100px,32vw,150px);

    animation:
    finalTeddy 1s infinite alternate;
}

@keyframes finalTeddy{

    from{
        transform:scale(1);
    }

    to{
        transform:scale(1.15);
    }
}

/* =========================
   EDITOR
========================= */

#editor{

    display:none;

    position:fixed;

    inset:0;

    z-index:2000;

    background:
    rgba(0,0,0,.65);

    padding:15px;

    align-items:center;

    justify-content:center;
}

.editorCard{

    width:100%;

    max-width:420px;

    max-height:90vh;

    overflow-y:auto;

    background:white;

    padding:25px;

    border-radius:25px;
}

.editorCard h2{

    color:#e93671;

    margin-bottom:15px;
}

.editorCard label{

    display:block;

    text-align:left;

    color:#777;

    font-size:13px;

    margin-top:13px;
}

.editorCard input,
.editorCard textarea{

    width:100%;

    padding:12px;

    margin-top:5px;

    border:2px solid #ffd0df;

    border-radius:13px;

    outline:none;
}

.editorCard textarea{

    min-height:80px;

    resize:vertical;
}

.saveButton{

    width:100%;

    padding:14px;

    margin-top:18px;

    background:#ed3572;

    color:white;

    border-radius:15px;

    font-weight:bold;
}

.closeButton{

    width:100%;

    padding:12px;

    margin-top:8px;

    background:#eee;

    border-radius:15px;
}

/* =========================
   SMALL SCREENS
========================= */

@media(max-width:380px){

    .page{
        padding-left:15px;
        padding-right:15px;
    }

    .photoFrame img{
        height:340px;
    }

    .memoryGrid img{
        height:145px;
    }

}

</style>
</head>

<body>


<!-- ==================================================
     LOGIN PAGE
================================================== -->

<section id="loginPage">

<div class="loginCard">

<div class="loginTeddy">
🧸
</div>

<h1>
A Little Surprise ❤️
</h1>

<p>
Enter your name and discover
10 special surprises.
</p>

<input
id="nameInput"
type="text"
placeholder="Enter your name..."
autocomplete="off">

<button
class="startButton"
onclick="startWebsite()">

Open My Surprise 🎁

</button>

</div>

</section>


<!-- ==================================================
     WEBSITE
================================================== -->

<div id="app">


<button
class="editButton"
onclick="openEditor()">

✏️ Edit

</button>


<!-- ==================================================
     SURPRISE 1
================================================== -->

<section
class="page active"
id="page1">

<div class="pageNumber">
1 / 10
</div>

<div class="content">

<h1 class="title">

Hey
<span class="personName">
You
</span>
💕

</h1>

<div class="speech">

🧸 "I love you more than
anything in this world!" ❤️

</div>

<div class="teddy">
🧸
</div>

<button
class="voiceButton"
onclick="teddySpeak()">

🔊 Teddy Speak

</button>

<p class="message">

Your first surprise
is waiting for you...

</p>

<button
class="nextButton"
onclick="nextPage()">

Open Surprise 2 💗

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 2
================================================== -->

<section
class="page"
id="page2">

<div class="pageNumber">
2 / 10
</div>

<div class="content">

<h1 class="title">
You Make My World Beautiful 🌎
</h1>

<div class="teddy">
🧸
</div>

<p
class="message"
id="message2">

Your smile can make
even an ordinary day beautiful.

</p>

<div style="font-size:45px;">
💕 ❤️ 💗 ❤️ 💕
</div>

<button
class="nextButton"
onclick="nextPage()">

Next Surprise 🎁

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 3
================================================== -->

<section
class="page"
id="page3">

<div class="pageNumber">
3 / 10
</div>

<div class="content">

<h1 class="title">
Your Beautiful Smile 🥰
</h1>

<div class="speech">

"Your smile is my
favourite feeling." 💗

</div>

<div class="teddy">
🧸
</div>

<p
class="message"
id="message3">

Never stop smiling.
Your happiness is precious.

</p>

<button
class="voiceButton"
onclick="speakText(
'Your smile is my favourite feeling!'
)">

🔊 Teddy Read

</button>

<br>

<button
class="nextButton"
onclick="nextPage()">

Next Surprise 💕

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 4 PHOTO
================================================== -->

<section
class="page"
id="page4">

<div class="pageNumber">
4 / 10
</div>

<div class="content">

<h1 class="title">
A Special Memory 📸
</h1>

<p class="message">
A picture especially for you.
</p>

<div class="photoFrame">

<img
src="photo1.jpg"
alt="Special memory">

</div>

<button
class="nextButton"
onclick="nextPage()">

Next Memory 💗

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 5 VIDEO
================================================== -->

<section
class="page"
id="page5">

<div class="pageNumber">
5 / 10
</div>

<div class="content">

<h1 class="title">
A Little Video 🎥
</h1>

<p class="message">
Press play for your special memory.
</p>

<div class="videoFrame">

<video
controls
playsinline>

<source
src="surprise.mp4"
type="video/mp4">

Your browser does not support video.

</video>

</div>

<p class="message">

Some moments deserve
to be remembered forever. ❤️

</p>

<button
class="nextButton"
onclick="nextPage()">

Next Surprise 🎁

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 6
================================================== -->

<section
class="page"
id="page6">

<div class="pageNumber">
6 / 10
</div>

<div class="content">

<h1 class="title">
You're One In A Million 💎
</h1>

<div class="teddy">
🧸
</div>

<p
class="message"
id="message6">

There is nobody exactly like you.
That's what makes you so special.

</p>

<div style="font-size:45px;">
✨ 💖 ✨ 💗 ✨
</div>

<button
class="nextButton"
onclick="nextPage()">

Another Surprise 💕

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 7 GIFT
================================================== -->

<section
class="page"
id="page7">

<div class="pageNumber">
7 / 10
</div>

<div class="content">

<h1 class="title">
A Gift For You 🎁
</h1>

<div
class="gift"
id="gift"
onclick="openGift()">

🎁

</div>

<p class="message">
Tap the gift box.
</p>

<div
class="giftMessage"
id="giftMessage">

Inside this box is
all my love for you. ❤️🧸

</div>

<button
class="nextButton"
onclick="nextPage()">

Next Surprise 💗

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 8 MEMORIES
================================================== -->

<section
class="page"
id="page8">

<div class="pageNumber">
8 / 10
</div>

<div class="content">

<h1 class="title">
Our Little Memories 📸
</h1>

<div class="memoryGrid">

<img
src="photo2.jpg"
alt="Memory 1">

<img
src="photo3.jpg"
alt="Memory 2">

<img
src="photo4.jpg"
alt="Memory 3">

<img
src="photo5.jpg"
alt="Memory 4">

</div>

<p class="message">

Every memory becomes
more beautiful because
you're part of it. 💕

</p>

<button
class="nextButton"
onclick="nextPage()">

One More Surprise 🎁

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 9
================================================== -->

<section
class="page"
id="page9">

<div class="pageNumber">
9 / 10
</div>

<div class="content">

<h1 class="title">
A Message From My Heart 💌
</h1>

<div class="speech">

<span id="message9">

You are the reason for
so many smiles,
beautiful memories
and happy moments.

</span>

<br><br>

❤️

</div>

<div class="teddy">
🧸
</div>

<button
class="voiceButton"
onclick="readMessage()">

🔊 Teddy Read This

</button>

<br>

<button
class="nextButton"
onclick="nextPage()">

Final Surprise ✨

</button>

</div>

</section>


<!-- ==================================================
     SURPRISE 10
================================================== -->

<section
class="page finalPage"
id="page10">

<div
class="pageNumber"
style="color:#e83270;">

10 / 10

</div>

<div class="content">

<h1 class="title">

My Final Surprise ❤️

</h1>

<div class="finalTeddy">
🧸
</div>

<p class="message">

<span class="personName">
You
</span>,

you are amazing,
special and deeply loved.

❤️

</p>

<div class="speech">

🧸 "I love you more
than words can explain." ❤️

</div>

<div style="font-size:45px;">
✨ 💕 🎆 💕 ✨
</div>

<button
class="nextButton"
style="
background:white;
color:#e83270;
"
onclick="restart()">

See Again 💕

</button>

</div>

</section>


</div>


<!-- ==================================================
     EDITOR
================================================== -->

<div id="editor">

<div class="editorCard">

<h2>
✏️ Edit Your Website
</h2>

<label>
Name
</label>

<input
id="editName"
type="text">


<label>
Surprise 2
</label>

<textarea
id="edit2">

Your smile can make
even an ordinary day beautiful.

</textarea>


<label>
Surprise 3
</label>

<textarea
id="edit3">

Never stop smiling.
Your happiness is precious.

</textarea>


<label>
Surprise 6
</label>

<textarea
id="edit6">

There is nobody exactly like you.
That's what makes you so special.

</textarea>


<label>
Surprise 9
</label>

<textarea
id="edit9">

You are the reason for so many smiles,
beautiful memories and happy moments.

</textarea>


<button
class="saveButton"
onclick="saveChanges()">

Save Changes ❤️

</button>

<button
class="closeButton"
onclick="closeEditor()">

Close

</button>

</div>

</div>


<script>

/* ==================================================
   VARIABLES
================================================== */

let currentPage=1;

let personName="You";


/* ==================================================
   START WEBSITE
================================================== */

function startWebsite(){

    const input=
    document
    .getElementById("nameInput");

    const name=
    input.value.trim();

    if(name===""){

        alert(
            "Please enter a name ❤️"
        );

        return;
    }

    personName=name;

    updateNames();

    document
    .getElementById("loginPage")
    .style.display="none";

    document
    .getElementById("app")
    .style.display="block";

    showPage(1);

    createHearts();

}


/* ==================================================
   UPDATE NAME
================================================== */

function updateNames(){

    document
    .querySelectorAll(".personName")
    .forEach(function(element){

        element.textContent=
        personName;

    });

}


/* ==================================================
   SHOW PAGE
================================================== */

function showPage(number){

    document
    .querySelectorAll(".page")
    .forEach(function(page){

        page.classList.remove("active");

    });

    const page=
    document.getElementById(
        "page"+number
    );

    if(page){

        page.classList.add("active");

    }

    currentPage=number;

    window.scrollTo(0,0);

    createHearts();

}


/* ==================================================
   NEXT PAGE
================================================== */

function nextPage(){

    if(currentPage<10){

        showPage(
            currentPage+1
        );

    }

}


/* ==================================================
   RESTART
================================================== */

function restart(){

    showPage(1);

}


/* ==================================================
   HEARTS
================================================== */

function createHearts(){

    const hearts=[
        "❤️",
        "💕",
        "💗",
        "💖",
        "💓",
        "💞",
        "🌸"
    ];

    for(
        let i=0;
        i<8;
        i++
    ){

        const heart=
        document.createElement("div");

        heart.className="heart";

        heart.textContent=
        hearts[
            Math.floor(
                Math.random()
                *hearts.length
            )
        ];

        heart.style.left=
        Math.random()*100+"vw";

        heart.style.fontSize=
        (18+
        Math.random()*25)
        +"px";

        heart.style.animationDuration=
        (4+
        Math.random()*4)
        +"s";

        document.body
        .appendChild(heart);

        setTimeout(
            function(){

                heart.remove();

            },
            8500
        );

    }

}


/* ==================================================
   VOICE
================================================== */

function teddySpeak(){

    speakText(
        "I love you more than anything in this world!"
    );

}

function speakText(text){

    if(
        !("speechSynthesis"
        in window)
    ){

        alert(
            "Voice is not supported by this browser."
        );

        return;
    }

    speechSynthesis.cancel();

    const speech=
    new SpeechSynthesisUtterance(
        text
    );

    speech.rate=.85;

    speech.pitch=1.3;

    speech.volume=1;

    speechSynthesis.speak(
        speech
    );

}


function readMessage(){

    const message=
    document
    .getElementById("message9")
    .innerText;

    speakText(message);

}


/* ==================================================
   GIFT
================================================== */

function openGift(){

    document
    .getElementById("gift")
    .textContent="💝";

    document
    .getElementById("giftMessage")
    .style.display="block";

    createHearts();

    speakText(
        "This gift contains all my love for you."
    );

}


/* ==================================================
   EDITOR
================================================== */

function openEditor(){

    document
    .getElementById("editor")
    .style.display="flex";

    document
    .getElementById("editName")
    .value=personName;

    document
    .getElementById("edit2")
    .value=
    document
    .getElementById("message2")
    .innerText;

    document
    .getElementById("edit3")
    .value=
    document
    .getElementById("message3")
    .innerText;

    document
    .getElementById("edit6")
    .value=
    document
    .getElementById("message6")
    .innerText;

    document
    .getElementById("edit9")
    .value=
    document
    .getElementById("message9")
    .innerText;

}


function closeEditor(){

    document
    .getElementById("editor")
    .style.display="none";

}


/* ==================================================
   SAVE EDITS
================================================== */

function saveChanges(){

    const name=
    document
    .getElementById("editName")
    .value
    .trim();

    if(name){

        personName=name;

        updateNames();

    }

    document
    .getElementById("message2")
    .innerText=
    document
    .getElementById("edit2")
    .value;

    document
    .getElementById("message3")
    .innerText=
    document
    .getElementById("edit3")
    .value;

    document
    .getElementById("message6")
    .innerText=
    document
    .getElementById("edit6")
    .value;

    document
    .getElementById("message9")
    .innerText=
    document
    .getElementById("edit9")
    .value;

    closeEditor();

}


/* ==================================================
   AUTO HEARTS
================================================== */

setInterval(
    function(){

        if(
            document
            .getElementById("app")
            .style.display==="block"
        ){

            createHearts();

        }

    },
    6000
);

</script>

</body>
</html>
