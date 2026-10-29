
<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CHARU ❤️ PIYUSH | Happy Karwa Chauth</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Tiro+Devanagari+Hindi&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background: linear-gradient(180deg, #3d0014, #800020, #25000b);
    color: #ffe9b0;
    font-family: 'Tiro Devanagari Hindi', serif;
    text-align: center;
    overflow-x: hidden;
    min-height: 100vh;
}

.stars {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 0;
}

.star {
    position: absolute;
    color: #ffe8a3;
    animation: twinkle 3s infinite alternate;
}

@keyframes twinkle {
    from { opacity: .2; transform: scale(.7); }
    to { opacity: 1; transform: scale(1.3); }
}

.container {
    position: relative;
    z-index: 1;
    max-width: 700px;
    margin: auto;
    padding: 35px 20px 60px;
}

.moon {
    width: 110px;
    height: 110px;
    border-radius: 50%;
    background: #fff1bd;
    box-shadow: 0 0 35px #ffe5a0, 0 0 100px #ffc76b;
    margin: 35px auto;
    position: relative;
}

.moon::after {
    content: "";
    position: absolute;
    width: 100px;
    height: 100px;
    background: #500017;
    border-radius: 50%;
    left: 25px;
    top: -10px;
}

h1 {
    font-family: 'Great Vibes', cursive;
    font-size: clamp(42px, 10vw, 70px);
    color: #ffd77c;
    text-shadow: 0 0 15px #ffb347;
    margin: 15px 0;
}

.subtitle {
    font-size: 20px;
    line-height: 1.8;
    margin: 20px auto;
}

.heart {
    color: #ff8a9e;
    font-size: 35px;
    animation: heartbeat 1.5s infinite;
}

@keyframes heartbeat {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
}

.card {
    background: rgba(255, 215, 128, .08);
    border: 1px solid #dca64a;
    border-radius: 25px;
    padding: 25px 20px;
    margin: 30px 0;
    box-shadow: 0 0 25px rgba(255, 180, 60, .12);
}

.card h2 {
    color: #ffd77c;
    margin-bottom: 18px;
    font-size: 25px;
}

.card p {
    font-size: 17px;
    line-height: 2;
}

button {
    background: linear-gradient(135deg, #ffd77c, #d99b35);
    color: #4a0014;
    border: none;
    border-radius: 30px;
    padding: 14px 25px;
    font-size: 17px;
    font-family: inherit;
    font-weight: bold;
    margin: 12px 5px;
    cursor: pointer;
    box-shadow: 0 5px 20px #0003;
}

button:active {
    transform: scale(.96);
}

.hidden {
    display: none;
}

#loveMessage {
    margin-top: 20px;
    line-height: 2;
    font-size: 18px;
    animation: appear 1s ease;
}

@keyframes appear {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.thali {
    font-size: 65px;
    margin: 15px;
}

footer {
    margin-top: 40px;
    font-size: 17px;
    line-height: 2;
    color: #ffd77c;
}

</style>
</head>

<body>

<div class="stars" id="stars"></div>

<div class="container">

    <div class="moon"></div>

    <h1>Happy Karwa Chauth</h1>

    <div class="heart">❤️</div>

    <p class="subtitle">
        मेरी प्यारी CHARU के लिए<br>
        एक छोटा-सा प्यार भरा तोहफ़ा 🌙
    </p>

    <div class="card">
        <div class="thali">🪔🌹🥮</div>

        <h2>मेरी चाँदनी CHARU</h2>

        <p>
            इस खूबसूरत चाँदनी रात में,<br>
            मेरी हर दुआ में बस तुम्हारा नाम है।<br>
            तुम मेरी ज़िंदगी की वो रोशनी हो,<br>
            जिसके बिना हर शाम अधूरी है।
        </p>
    </div>

    <div class="card">
        <h2>💌 तुम्हारे लिए एक ख़त</h2>

        <p>
            मेरी प्यारी CHARU,<br><br>

            करवा चौथ का ये खूबसूरत त्योहार
            मुझे तुम्हारी याद दिलाता है।
            चाँद की तरह तुम मेरी ज़िंदगी में
            रोशनी और सुकून लेकर आती हो।<br><br>

            तुम्हारी मुस्कान मेरी सबसे प्यारी खुशी है।
            मेरी बस यही दुआ है कि तुम्हारी ज़िंदगी
            हमेशा खुशियों से भरी रहे।<br><br>

            तुम्हारा साथ मेरे लिए बहुत खास है।
            आज और हमेशा तुम्हारे चेहरे पर
            मुस्कान बनी रहे। ❤️
        </p>

        <div class="heart">❤️</div>

        <p>
            हमेशा तुम्हारा,<br>
            <b>PIYUSH</b>
        </p>
    </div>

    <div class="card">

        <h2>🌙 मेरे दिल की बात</h2>

        <p>
            CHARU, एक बात कहूँ?
        </p>

        <button onclick="showLove()">
            हाँ, कहो ❤️
        </button>

        <div id="loveMessage" class="hidden">
            तुम मेरी ज़िंदगी का सबसे प्यारा हिस्सा हो।<br>
            तुम्हारे साथ हर पल खास लगता है।<br>
            मेरी हर छोटी-बड़ी खुशी में<br>
            तुम्हारा नाम शामिल है।<br><br>

            <span style="font-size:30px">I LOVE YOU CHARU ❤️</span>
        </div>

    </div>

    <div class="card">

        <h2>✨ एक प्यारी-सी दुआ</h2>

        <p>
            चाँद की चाँदनी तुम्हारे चेहरे पर रहे,<br>
            खुशियों की रोशनी तुम्हारी ज़िंदगी में रहे।<br>
            हर दिन तुम्हारे लिए खूबसूरत हो,<br>
            और तुम्हारी हर मुस्कान सलामत रहे।
        </p>

    </div>

    <button onclick="createHearts()">
        ढेर सारा प्यार भेजो ❤️
    </button>

    <footer>
        Made with ❤️ by PIYUSH<br>
        सिर्फ मेरी CHARU के लिए 🌙
    </footer>

</div>

<script>

// सितारों का एनिमेशन
const stars = document.getElementById("stars");

for (let i = 0; i < 80; i++) {
    const star = document.createElement("div");
    star.className = "star";
    star.innerHTML = "✦";

    star.style.left = Math.random() * 100 + "%";
    star.style.top = Math.random() * 100 + "%";
    star.style.fontSize = (Math.random() * 12 + 5) + "px";
    star.style.animationDelay = Math.random() * 3 + "s";

    stars.appendChild(star);
}

// लव मैसेज
function showLove() {
    const message = document.getElementById("loveMessage");

    message.classList.remove("hidden");

    message.scrollIntoView({
        behavior: "smooth",
        block: "center"
    });
}

// दिलों की बारिश
function createHearts() {
    for (let i = 0; i < 30; i++) {
        const heart = document.createElement("div");

        heart.innerHTML = "❤️";
        heart.style.position = "fixed";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.top = "-30px";
        heart.style.fontSize = (Math.random() * 25 + 15) + "px";
        heart.style.zIndex = "999";
        heart.style.pointerEvents = "none";

        document.body.appendChild(heart);

        const duration = Math.random() * 3 + 2;

        heart.animate([
            { transform: "translateY(0)", opacity: 1 },
            { transform: "translateY(100vh)", opacity: 0 }
        ], {
            duration: duration * 1000,
            easing: "ease-in"
        });

        setTimeout(() => heart.remove(), duration * 1000);
    }
}

</script>

</body>
</html>
