<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

<title>101 Reasons Why I Love You ♡</title>


<style>

/* =====================================================
   RESET
===================================================== */

* {
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {

    margin: 0;

    min-height: 100vh;

    font-family:
        Georgia,
        "Times New Roman",
        serif;

    color: #fff4f5;

    overflow-x: hidden;

    background:
        radial-gradient(
            circle at 50% 15%,
            #7c2639 0%,
            #551527 25%,
            #320b1a 55%,
            #18050d 80%,
            #090207 100%
        );

}


/* =====================================================
   STARS
===================================================== */

.stars {

    position: fixed;

    inset: 0;

    z-index: 0;

    pointer-events: none;

    background-image:

        radial-gradient(
            2px 2px at 10% 20%,
            #ffe8ec,
            transparent
        ),

        radial-gradient(
            1px 1px at 20% 70%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 30% 40%,
            #ffd4dc,
            transparent
        ),

        radial-gradient(
            1px 1px at 40% 80%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 50% 15%,
            #ffe0e6,
            transparent
        ),

        radial-gradient(
            1px 1px at 60% 60%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 70% 30%,
            #ffd6de,
            transparent
        ),

        radial-gradient(
            1px 1px at 80% 75%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 90% 45%,
            #ffe8ec,
            transparent
        );

    background-size: 350px 350px;

    animation:
        starsMove 35s linear infinite;

    opacity: .75;

}


.stars::after {

    content: "";

    position: absolute;

    inset: 0;

    background-image:

        radial-gradient(
            1px 1px at 15% 50%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 45% 25%,
            #ffd5dd,
            transparent
        ),

        radial-gradient(
            1px 1px at 65% 85%,
            #ffffff,
            transparent
        ),

        radial-gradient(
            2px 2px at 85% 15%,
            #ffe8ec,
            transparent
        );

    background-size: 250px 250px;

    animation:
        starsMoveReverse 50s linear infinite;

    opacity: .45;

}


@keyframes starsMove {

    from {
        transform:
            translate(0, 0);
    }

    to {
        transform:
            translate(-150px, -120px);
    }

}


@keyframes starsMoveReverse {

    from {
        transform:
            translate(0, 0);
    }

    to {
        transform:
            translate(130px, 100px);
    }

}


/* =====================================================
   FLOATING HEARTS
===================================================== */

.heart {

    position: fixed;

    bottom: -40px;

    z-index: 1;

    color: #e99cab;

    font-size: 18px;

    opacity: 0;

    pointer-events: none;

    animation:
        floatingHeart
        linear
        infinite;

}


@keyframes floatingHeart {

    0% {

        transform:
            translateY(0)
            rotate(0deg);

        opacity: 0;

    }

    15% {

        opacity: .65;

    }

    80% {

        opacity: .5;

    }

    100% {

        transform:
            translateY(-110vh)
            rotate(35deg);

        opacity: 0;

    }

}


/* =====================================================
   MAIN CONTAINER
===================================================== */

.container {

    position: relative;

    z-index: 5;

    width:
        min(1050px, 92%);

    margin:
        0 auto;

    padding:
        70px 0 100px;

    text-align:
        center;

}


/* =====================================================
   HEADER
===================================================== */

.small-title {

    font-size:
        13px;

    letter-spacing:
        5px;

    text-transform:
        uppercase;

    color:
        #e8a0ad;

    opacity:
        .75;

}


h1 {

    margin:
        12px 0 5px;

    font-size:
        clamp(40px, 7vw, 70px);

    font-weight:
        normal;

    letter-spacing:
        2px;

    color:
        #fff5f6;

    text-shadow:

        0 0 12px
        rgba(255, 190, 205, .45),

        0 0 35px
        rgba(170, 45, 70, .5);

}


.subtitle {

    margin-top:
        10px;

    font-size:
        17px;

    color:
        #edb5c0;

    opacity:
        .9;

}


.counter {

    display:
        inline-block;

    margin-top:
        22px;

    padding:
        9px 20px;

    border:
        1px solid
        rgba(235, 155, 175, .25);

    border-radius:
        30px;

    background:
        rgba(90, 18, 38, .4);

    color:
        #f2c2ca;

    font-size:
        13px;

    box-shadow:
        0 5px 20px
        rgba(0,0,0,.15);

}


/* =====================================================
   REASONS GRID
===================================================== */

.reasons {

    display:
        grid;

    grid-template-columns:
        repeat(5, 1fr);

    gap:
        14px;

    margin-top:
        45px;

}


/* =====================================================
   REASON BUTTON
===================================================== */

.reason {

    position:
        relative;

    min-height:
        105px;

    border:
        1px solid
        rgba(220, 125, 145, .22);

    border-radius:
        18px;

    background:
        linear-gradient(
            145deg,
            rgba(110, 31, 52, .72),
            rgba(42, 8, 22, .86)
        );

    color:
        #fff4f5;

    cursor:
        pointer;

    font-family:
        Georgia,
        "Times New Roman",
        serif;

    transition:
        transform .25s ease,
        box-shadow .25s ease,
        border-color .25s ease,
        background .25s ease;

    overflow:
        hidden;

}


.reason::before {

    content:
        "♡";

    position:
        absolute;

    right:
        10px;

    top:
        6px;

    font-size:
        13px;

    color:
        #eaa1ae;

    opacity:
        .35;

}


.reason:hover {

    transform:
        translateY(-7px)
        scale(1.03);

    border-color:
        rgba(245, 165, 180, .6);

    background:
        linear-gradient(
            145deg,
            rgba(140, 44, 68, .85),
            rgba(52, 10, 27, .95)
        );

    box-shadow:

        0 15px 30px
        rgba(0,0,0,.4),

        0 0 25px
        rgba(175, 45, 70, .25);

}


.reason:active {

    transform:
        scale(.96);

}


.number {

    display:
        block;

    margin-bottom:
        7px;

    font-size:
        25px;

    font-weight:
        bold;

    color:
        #f0b7c1;

}


.tap {

    display:
        block;

    font-size:
        10px;

    letter-spacing:
        1.5px;

    text-transform:
        uppercase;

    color:
        #d997a5;

    opacity:
        .75;

}


/* =====================================================
   MODAL BACKGROUND
===================================================== */

.modal {

    position:
        fixed;

    inset:
        0;

    z-index:
        100;

    display:
        flex;

    align-items:
        center;

    justify-content:
        center;

    padding:
        25px;

    background:
        rgba(18, 2, 8, .88);

    backdrop-filter:
        blur(10px);

    opacity:
        0;

    pointer-events:
        none;

    transition:
        opacity .3s ease;

}


.modal.show {

    opacity:
        1;

    pointer-events:
        auto;

}


/* =====================================================
   POPUP CARD
===================================================== */

.reason-card {

    position:
        relative;

    width:
        min(540px, 100%);

    padding:
        52px 42px 42px;

    text-align:
        center;

    border:
        1px solid
        rgba(235, 155, 175, .45);

    border-radius:
        28px;

    background:
        linear-gradient(
            145deg,
            #681d34,
            #280815
        );

    box-shadow:

        0 30px 90px
        rgba(0,0,0,.65),

        0 0 50px
        rgba(170, 40, 65, .25);

    transform:
        scale(.8)
        translateY(25px);

    transition:
        transform .35s ease;

}


.modal.show .reason-card {

    transform:
        scale(1)
        translateY(0);

}


.reason-card::before {

    content:
        "♡";

    position:
        absolute;

    top:
        18px;

    right:
        25px;

    color:
        #e7a0ad;

    font-size:
        25px;

    opacity:
        .6;

}


.reason-number {

    font-size:
        13px;

    letter-spacing:
        4px;

    text-transform:
        uppercase;

    color:
        #e4a0ad;

    opacity:
        .8;

}


.reason-card h2 {

    margin:
        15px 0 25px;

    font-size:
        38px;

    font-weight:
        normal;

    color:
        #f4b8c2;

}


.reason-message {

    min-height:
        80px;

    font-size:
        clamp(17px, 3vw, 21px);

    line-height:
        1.8;

    color:
        #fff0f2;

}


/* =====================================================
   CLOSE BUTTON
===================================================== */

.close {

    margin-top:
        30px;

    padding:
        11px 28px;

    border:
        none;

    border-radius:
        25px;

    background:
        #9e3b55;

    color:
        white;

    font-family:
        Georgia,
        "Times New Roman",
        serif;

    cursor:
        pointer;

    transition:
        .2s ease;

    box-shadow:
        0 5px 18px
        rgba(0,0,0,.25);

}


.close:hover {

    transform:
        scale(1.06);

    background:
        #b94c68;

    box-shadow:
        0 0 22px
        rgba(210,75,105,.35);

}


/* =====================================================
   FINAL MESSAGE
===================================================== */

.final-message {

    margin-top:
        65px;

    padding:
        35px 25px;

    border-top:
        1px solid
        rgba(225, 140, 160, .2);

    border-bottom:
        1px solid
        rgba(225, 140, 160, .2);

}


.heart-big {

    font-size:
        38px;

    color:
        #e5a0ae;

    text-shadow:
        0 0 20px
        rgba(220, 75, 110, .45);

    animation:
        heartbeat 1.8s ease-in-out infinite;

}


@keyframes heartbeat {

    0%,
    100% {

        transform:
            scale(1);

    }

    50% {

        transform:
            scale(1.15);

    }

}


.final-message p {

    max-width:
        650px;

    margin:
        15px auto 0;

    line-height:
        1.8;

    color:
        #edc1c8;

    opacity:
        .85;

}


/* =====================================================
   FOOTER
===================================================== */

footer {

    margin-top:
        45px;

    font-size:
        12px;

    letter-spacing:
        2px;

    color:
        #d995a3;

    opacity:
        .55;

}


/* =====================================================
   MOBILE
===================================================== */

@media(max-width: 850px) {

    .reasons {

        grid-template-columns:
            repeat(4, 1fr);

    }

}


@media(max-width: 600px) {

    .container {

        padding-top:
            50px;

    }

    .reasons {

        grid-template-columns:
            repeat(3, 1fr);

        gap:
            10px;

    }

    .reason {

        min-height:
            90px;

        border-radius:
            14px;

    }

    .number {

        font-size:
            20px;

    }

    .tap {

        font-size:
            9px;

    }

    .reason-card {

        padding:
            42px 25px 30px;

    }

}


@media(max-width: 400px) {

    .reasons {

        grid-template-columns:
            repeat(2, 1fr);

    }

}


/* =====================================================
   ACCESSIBILITY
===================================================== */

button:focus-visible {

    outline:
        2px solid
        #f2a8b7;

    outline-offset:
        3px;

}

</style>

</head>


<body>


<!-- =====================================================
     BACKGROUND
===================================================== -->

<div class="stars"></div>


<!-- =====================================================
     FLOATING HEARTS
===================================================== -->

<div class="heart"
     style="
        left: 7%;
        animation-duration: 13s;
        animation-delay: 1s;
     ">
    ♡
</div>

<div class="heart"
     style="
        left: 19%;
        animation-duration: 17s;
        animation-delay: 4s;
     ">
    ♥
</div>

<div class="heart"
     style="
        left: 34%;
        animation-duration: 14s;
        animation-delay: 2s;
     ">
    ♡
</div>

<div class="heart"
     style="
        left: 51%;
        animation-duration: 19s;
        animation-delay: 6s;
     ">
    ♥
</div>

<div class="heart"
     style="
        left: 67%;
        animation-duration: 15s;
        animation-delay: 3s;
     ">
    ♡
</div>

<div class="heart"
     style="
        left: 81%;
        animation-duration: 18s;
        animation-delay: 5s;
     ">
    ♥
</div>

<div class="heart"
     style="
        left: 94%;
        animation-duration: 12s;
        animation-delay: 7s;
     ">
    ♡
</div>


<!-- =====================================================
     MAIN
===================================================== -->

<div class="container">


    <!-- HEADER -->

    <div class="small-title">
        a little list for you
    </div>


    <h1>
        100 Reasons
    </h1>


    <div class="subtitle">
        Why I Love You ♡
    </div>


    <div
        class="counter"
        id="counter"
    >
        0 / 100 reasons discovered
    </div>


    <!-- REASONS -->

    <div
        class="reasons"
        id="reasons"
    ></div>


    <!-- FINAL MESSAGE -->

    <div class="final-message">

        <div class="heart-big">
            ♡
        </div>

        <p>
            You can count them, but honestly,
            I appreciate you, more than these 101 reasons I listed, and more than I have ever said.
        </p>

    </div>


    <footer>
        made with love, basta ikaw ♡
    </footer>


</div>


<!-- =====================================================
     POPUP
===================================================== -->

<div
    class="modal"
    id="modal"
>

    <div class="reason-card">


        <div
            class="reason-number"
            id="reasonNumber"
        >
            reason 01
        </div>


        <h2>
            ♡
        </h2>


        <div
            class="reason-message"
            id="reasonMessage"
        >
            Message
        </div>


        <button
            class="close"
            onclick="closeReason()"
        >
            close ♡
        </button>


    </div>

</div>


<script>


/* =====================================================
   100 REASONS
===================================================== */

const reasons = [

    "I love how understanding you are.",

    "I love how you make me smile, and laugh.",

    "I love talking to you, it makes me sooo happy !!",

    "I love the way you listen to me, even the smallest things, and utter nonsense.",

    "I love how you put effort into our relationship, even if we aren't exactly dating yet.",

    "I love how patient you can be with me.",

    "I love you, kahit wala kang sense of humor, you still try to.",

    "I love all the little things you do.",

    "I love how you gave me a jacket and still letting me borrow.",

    "I love how comfortable I feel talking to you.",

    "I love the way how we fight, we fix, and we stay.",

    "I love your dedication, even when I'm pushng you away.",

    "I love how I can be comfortable around you without thinking about how you'll be turned off.",

    "I love how you support me.",

    "I love that I can be myself around you.",

    "I love our random conversations.",

    "I love our inside jokes, especially the freaky ones.",

    "I love remembering our funny moments, I SEE YOU VOLLEYBALL LEGENDS",

    "I love the way you still get me something from 7/11 even though you're running late.",

    "I love that every memory with you feels special.",

    "I love how you try to understand my yapping about Greek Mythology.",

    "I love how you put up with my random moods.",

    "I love how you make me feel appreciated.",

    "I love how honest you are with me, even though it hurts.",

    "I love how you buy me food in the canteen during your breaktimes.",

    "I love how genuine you are.",

    "I love how you can make a boring day better.",

    "I love hearing from you.",

    "I love seeing your messages pop up.",

    "I love how one conversation with you can change my mood.",

    "I love how we can joke around together.",

    "I love how we can also talk seriously when we need to.",

    "I love how you don't have to pretend around me.",

    "I love that I can trust you.",

    "I love how much we've learned about each other.",

    "I love discovering new things about you.",

    "I love your favorite songs, the songs you tell me to listen to.",

    "I love how you don't curse me out when you're mad at me.",

    "I love how you make me feel less alone.",

    "I love how you make me feel heard.",

    "I love how you spoil me with food, gifts, and things I wan't.",

    "I love seeing you excited about things you enjoy.",

    "I love hearing you talk about things you're interested in.",

    "I love seeing you happy.",

    "I love your determination, especially when you had to transfer to my school just to see me when you're 2 hours away.(not sure if this is dedication or determination hehe)",

    "I love how you keep going when things get difficult.",

    "I love the fact that you make my sad day better.",

    "I love our silly moments.",

    "I love our serious moments.",

    "I love our chaotic moments.",

    "I love our peaceful moments.",

    "I love the fact that you made me want to live life again.",

    "I love simply spending time talking with you.",

    "I love how much I look forward to hearing from you.",

    "I love how you make me excited about the future.",

    "I love imagining all the things we could experience together.",

    "I love having someone I can share things with.",

    "I love telling you about my day.",

    "I love hearing about yours= day.",

    "I love how our conversations can go from serious to completely random.",

    "I love when we walk home from school together.",

    "I love that you know how to cheer me up.",

    "I love how you can tell when something is bothering me.",

    "I love how you care.",

    "I love when we eat mcdo, kalye wings, whatever we buy together.",

    "I love the effort you put into making things meaningful.",

    "I love that you are uniquely you.",

    "I love how you make me feel loved.",

    "I love the way you think of ways to see me.",

    "I love how you don't make me feel like my feeling are invalid.",

    "I love learning from you.",

    "I love how you make me think about things differently.",

    "I love how you can surprise me.",

    "I love the little things that remind me of you.",

    "I love how many memories in the future already make me think of you.",

    "I love how you became such an important part of my life in just 4 months.",

    "I love how much I care about you.",

    "I love how happy your happiness can make me.",

    "I love celebrating your little wins.",

    "I love being able to encourage you.",

    "I love knowing I can be there for you.",

    "I love how we can grow and learn together.",

    "I love the things we've experienced together.",

    "I love the stories we already have.",

    "I love that there are still so many memories to make ahead.",

    "I love how you make me appreciate the little moments.",

    "I love how you push me to become better together than just leaving me alone.",

    "I love how you listen to my gibberish yapping.",

    "I love the comfort of knowing you're there.",

    "I love how you make me feel cared for.",

    "I love how you make me want to be better.",

    "I love how you inspire me.",

    "I love how much I appreciate having you in my life.",

    "I love how you respect my boundaries.",

    "I love you for all the reasons I can explain.",

    "I love you for all the reasons I can't explain.",

    "I love that you make my days a little brighter.",

    "I love that I have someone that I can confide to.",

    "I love you because you're you.",

    "I love that after all these reasons, I could still keep going. ♡",

    "I love you above all, to the stars and beyond, gelo."
];


/* =====================================================
   CREATE ALL 100 BUTTONS
===================================================== */

const reasonsContainer =
    document.getElementById("reasons");

const counter =
    document.getElementById("counter");

const modal =
    document.getElementById("modal");

const reasonNumber =
    document.getElementById("reasonNumber");

const reasonMessage =
    document.getElementById("reasonMessage");


let discovered = 0;

const discoveredReasons =
    new Set();


reasons.forEach(
    (reason, index) => {


        const button =
            document.createElement("button");


        button.className =
            "reason";


        button.type =
            "button";


        button.innerHTML = `

            <span class="number">
                ${String(index + 1).padStart(2, "0")}
            </span>

            <span class="tap">
                tap to open ♡
            </span>

        `;


        button.addEventListener(
            "click",
            () => {

                openReason(index);

            }
        );


        reasonsContainer.appendChild(
            button
        );


    }
);


/* =====================================================
   OPEN REASON
===================================================== */

function openReason(index) {


    reasonNumber.textContent =
        `reason ${String(index + 1).padStart(2, "0")}`;


    reasonMessage.textContent =
        reasons[index];


    modal.classList.add(
        "show"
    );


    if (
        !discoveredReasons.has(index)
    ) {

        discoveredReasons.add(
            index
        );


        discovered++;


        counter.textContent =
            `${discovered} / 100 reasons discovered`;

    }

}


/* =====================================================
   CLOSE REASON
===================================================== */

function closeReason() {

    modal.classList.remove(
        "show"
    );

}


/* =====================================================
   CLICK OUTSIDE
===================================================== */

modal.addEventListener(
    "click",
    function(event) {

        if (
            event.target === modal
        ) {

            closeReason();

        }

    }
);


/* =====================================================
   ESCAPE KEY
===================================================== */

document.addEventListener(
    "keydown",
    function(event) {

        if (
            event.key === "Escape"
        ) {

            closeReason();

        }

    }
);


</script>


</body>

</html>
