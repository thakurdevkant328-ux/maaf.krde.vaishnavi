<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Vaishnavi ❤️</title>
<style>
    /* --- IMPORT FONTS --- */
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Dancing+Script:wght@600&display=swap');

    :root {
        --primary-color: #ff4d6d;
        --bg-color: #fff0f3;
        --chat-bg: #e5ddd5;
        --sent-bg: #dcf8c6;
    }

    /* --- 1. CAT PAW CURSOR --- */
    body {
        margin: 0;
        font-family: 'Poppins', sans-serif;
        background: var(--bg-color);
        color: #333;
        overflow-x: hidden;
        /* Cute Cat Paw Cursor Link */
        cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), auto; 
    }

    /* Hover effect ke liye bhi same cursor */
    a, button, .jar-container, .gift-box, input[type=range] {
        cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), pointer;
    }

    /* --- 2. FLOATING HEARTS BACKGROUND --- */
    .bg-hearts {
        position: fixed;
        top: 0; left: 0; width: 100%; height: 100%;
        overflow: hidden;
        z-index: -1;
        pointer-events: none;
    }
    .heart-bg {
        position: absolute;
        bottom: -10px;
        color: rgba(255, 77, 109, 0.2);
        animation: floatUp 10s linear infinite;
        font-size: 20px;
    }
    @keyframes floatUp {
        0% { transform: translateY(0) rotate(0deg); opacity: 1; }
        100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
    }

    /* --- OVERLAY --- */
    #start-overlay {
        position: fixed; top: 0; left: 0; width: 100%; height: 100%;
        background: #000;
        display: flex; justify-content: center; align-items: center;
        z-index: 9999; color: white; flex-direction: column;
    }
    #start-btn {
        padding: 15px 30px; background: var(--primary-color);
        border: none; color: white; font-size: 18px; border-radius: 50px;
        margin-top: 20px; animation: pulse 2s infinite;
    }

    section {
        padding: 40px 20px; max-width: 600px; margin: auto;
        text-align: center; background: white; margin-bottom: 20px;
        border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        position: relative; z-index: 1;
    }

    h1 { color: var(--primary-color); margin-bottom: 5px; }
    h2 { color: #444; margin-top: 0; }
    p { font-size: 16px; line-height: 1.6; color: #666; }

    /* TEXT BOXES */
    .text-content {
        text-align: left; background: #fafafa; padding: 20px;
        border-radius: 10px; border-left: 5px solid var(--primary-color);
        margin-bottom: 10px;
    }
    .highlight { background-color: #fff3cd; padding: 2px 5px; border-radius: 4px; font-weight: 600; }

    /* POETRY STYLE */
    .poetry-box {
        font-family: 'Dancing Script', cursive; font-size: 22px; line-height: 1.8;
        color: #d63384; background: #fff0f3; padding: 20px;
        border-radius: 15px; border: 1px dashed var(--primary-color);
    }

    /* TIMER */
    .timer-box {
        font-size: 18px; font-weight: bold; color: #555; background: #fff;
        padding: 15px; border: 2px dashed var(--primary-color); border-radius: 10px;
    }

    /* MOOD SLIDER */
    .slider-container { margin: 20px 0; }
    input[type=range] { width: 100%; accent-color: var(--primary-color); }
    #mood-text { font-weight: bold; margin-top: 10px; color: var(--primary-color); }

    /* CHAT INTERFACE */
    .chat-container {
        background: var(--chat-bg); padding: 15px; border-radius: 15px;
        height: 300px; overflow-y: auto; display: flex; flex-direction: column;
        border: 1px solid #ddd;
    }
    .msg {
        max-width: 80%; padding: 8px 12px; margin: 5px 0; border-radius: 10px;
        font-size: 14px; position: relative; opacity: 0; transform: translateY(10px);
        transition: all 0.5s ease;
    }
    .msg.show { opacity: 1; transform: translateY(0); }
    .sent { background: var(--sent-bg); align-self: flex-end; border-bottom-right-radius: 0; }

    /* PROMISE JAR */
    .jar-container { cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), pointer; transition: transform 0.3s; }
    .jar-container:active { transform: scale(0.95); }
    .jar-icon { font-size: 60px; }
    .promise-card {
        margin-top: 15px; padding: 15px; background: #fffbeb;
        border: 1px solid #ffd700; border-radius: 10px; display: none; animation: fadeIn 0.5s;
    }

    /* GALLERY */
    .gallery { display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; }
    .gallery img { width: 100%; border-radius: 10px; object-fit: cover; box-shadow: 0 4px 8px rgba(0,0,0,0.1); }

    /* COUPON */
    .gift-box { font-size: 60px; cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), pointer; animation: bounce 2s infinite; }
    .coupon { display: none; background: #fff; border: 2px dashed #333; padding: 20px; margin-top: 20px; }

    /* WHATSAPP BTN */
    .whatsapp-btn {
        position: fixed; bottom: 20px; right: 20px;
        background: #25d366; color: white; padding: 12px 20px;
        border-radius: 50px; text-decoration: none; font-weight: bold;
        box-shadow: 0 4px 10px rgba(0,0,0,0.3); display: none; z-index: 1000;
        cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), pointer;
    }

    /* ANIMATIONS */
    @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.1); } 100% { transform: scale(1); } }
    @keyframes bounce { 0%, 20%, 50%, 80%, 100% {transform: translateY(0);} 40% {transform: translateY(-10px);} 60% {transform: translateY(-5px);} }
    @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
    
    /* CONFETTI */
    .confetti { position: fixed; width: 10px; height: 10px; background: red; top: -10px; z-index: 999; animation: fall 3s linear infinite; }
    @keyframes fall { to { top: 100vh; transform: rotate(360deg); } }

</style>
</head>
<body>

    <div class="bg-hearts" id="bg-hearts"></div>

    <div id="start-overlay">
        <h1>For Vaishnavi ❤️</h1>
        <p>Please turn up your volume.</p>
        <button id="start-btn" onclick="startExperience()">Open My Heart</button>
    </div>

    <div id="main-content" style="display:none;">
        
        <section>
            <h1>I'm Sorry.</h1>
            <p>I messed up, and I want to fix it.</p>
            
            <div class="slider-container">
                <p>How angry are you right now?</p>
                <input type="range" min="0" max="100" value="100" id="moodRange" oninput="updateMood()">
                <div id="mood-text">😡 I am furious!</div>
            </div>
        </section>

        <section>
            <h2>⏳ Time Since 2nd Aug 2025</h2>
            <div class="timer-box" id="timer">Calculating...</div>
        </section>

        <section>
            <h2>💬 Just Listen Once?</h2>
            <div class="chat-container" id="chat-box"></div>
        </section>

        <section>
            <h2>😔 My Confession</h2>
            <div class="text-content">
                <p>My Dear Vaishnavi,</p>
                <p>I know maine galti ki hai aur main apni saari galti accept karta hoon. Please Vaishnavi mujhe maaf kar do. Mera intention kabhi bhi tumhe hurt karna nahi tha.</p>
                <p>Main tere rude behaviour se gusse mein aa gaya tha, lekin mujhe pata hai mujhe aisa nahi karna chahiye tha. <span class="highlight">Teri story pe Anush ka comment dekh ke main sach mein toot gaya tha.</span></p>
                <p>Maine <span class="highlight">Antrika</span> ke saath koi chugli nahi ki thi. Main sirf itna kehne gaya tha ki apne bf ko control kare. Uske baad main tumse baat karna chahta tha, lekin tera behaviour mujhe bahut zyada hurt kar gaya.</p>
                <p>Meri wajah se agar teri friendship toot gayi ho, toh main dil se maafi maangta hoon.</p>
                <p><b>Please Vaishnavi, ek last chance de do. I swear, I will treat you like a queen. 👑</b></p>
            </div>
        </section>

        <section>
            <h2>💌 A Letter From My Heart</h2>
            <div class="text-content">
                <p><b>My Dearest Vaishnavi,</b></p>
                <p>I am writing this to you because sometimes my spoken words fail to express the depth of what I truly feel in my heart. I know things have been difficult between us lately, and the thought that I might be the reason for your sadness kills me inside. But I want you to know one thing with absolute certainty: <b>you are the most beautiful part of my life.</b></p>
                <p>Before you, I was just existing, but with you, I started living. You are not just my girlfriend; you are my best friend, my safe place, and the only person who truly understands me. I know I am not perfect. I make mistakes, and sometimes I say things I don't mean, but never for a second doubt my love for you.</p>
                <p>I promise you, Vaishnavi, that I am here for the long run. I want to fix this, not just for today, but because I cannot imagine a future that doesn't have you in it.</p>
                <p>Please let go of this anger and look at me—you will see a boy who is hopelessly in love with you and is willing to do whatever it takes to see you smile again.</p>
                <p>I love you more than words can say, and I will keep loving you until my very last breath. You are my forever. 💐🛐</p>
            </div>
        </section>

        <section>
            <h2>🌹 For You</h2>
            <div class="poetry-box">
                I miss the smile upon your face,<br>
                I miss your warm and loving embrace.<br>
                I know I made you feel meaningful pain,<br>
                And I promise not to do it again.<br><br>
                Life without you is hard to bear,<br>
                I look for you everywhere.<br>
                Please forget the fights we had,<br>
                Being apart makes me so sad.<br><br>
                Vaishnavi, you are my heart and soul,<br>
                Only you can make me whole.<br>
                Please come back and hold my hand,<br>
                Let's build the life that we had planned.<br><br>
                I love you more than words can say,<br>
                I miss you every single day. ❤️
            </div>
        </section>

        <section>
            <h2>🏺 The Promise Jar</h2>
            <p>Tap the jar to see my promises to you.</p>
            <div class="jar-container" onclick="showPromise()">
                <div class="jar-icon">🏺</div>
            </div>
            <div class="promise-card" id="promise-display"></div>
        </section>

        <section>
            <h2>📸 Us</h2>
            <div class="gallery">
                <img src="https://i.ibb.co/WvZCqXrJ/f050c675-8b43-4e06-be87-a6d71669c771-d146cfb7-252f-48cb-ba3c-9da826f0f173-2.jpg">
                <img src="https://i.ibb.co/xbLT1BP/Screenshot-20251227-063846-Photos.jpg">
                <img src="https://i.ibb.co/Txmdv3Kr/Screenshot-20251227-145012-Gallery.jpg">
                <img src="https://i.ibb.co/RkN4dd2P/Screenshot-20251227-145038-Gallery.jpg">
            </div>
        </section>

        <section>
            <h2>🎁 Peace Offering</h2>
            <div class="gift-box" onclick="openCoupon()">🎁</div>
            <div class="coupon" id="coupon">
                <h3>Coupon Code: LOVE2025</h3>
                <p><b>Valid for:</b> One long hug 🫂 & Unlimited Momos 🥟</p>
                <p style="font-size:12px;">Redeemable anytime. Lifetime validity.</p>
            </div>
        </section>

        <a href="https://wa.me/919369068575" class="whatsapp-btn" id="wa-btn">Reply? 💬</a>

    </div>

    <audio id="bg-music" loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3">
    </audio>

<script>
    // --- CREATE FLOATING HEARTS ---
    function createHearts() {
        const container = document.getElementById('bg-hearts');
        for(let i=0; i<15; i++) {
            let heart = document.createElement('div');
            heart.innerHTML = '❤️';
            heart.className = 'heart-bg';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 5 + 5) + 's';
            heart.style.fontSize = (Math.random() * 20 + 10) + 'px';
            container.appendChild(heart);
        }
    }
    createHearts(); // Run on load

    // START
    function startExperience() {
        document.getElementById('start-overlay').style.display = 'none';
        document.getElementById('main-content').style.display = 'block';
        document.getElementById('bg-music').volume = 0.5;
        document.getElementById('bg-music').play();
        startChat();
    }

    // --- TIMER UPDATED TO 2 AUGUST 2025 ---
    // Month is 0-indexed (Jan=0, Aug=7)
    const startDate = new Date(2025, 7, 2); 
    
    setInterval(() => {
        const now = new Date();
        const diff = now - startDate;
        
        // Agar future date hai to 0 dikhayega
        if (diff < 0) {
            document.getElementById("timer").innerText = "Timer will start on Aug 2, 2025";
            return;
        }

        const days = Math.floor(diff / (1000 * 60 * 60 * 24));
        const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        
        document.getElementById("timer").innerText = 
            `${days} Days, ${hours} Hours, ${minutes} Minutes`;
    }, 1000);

    // MOOD
    function updateMood() {
        const val = document.getElementById('moodRange').value;
        const text = document.getElementById('mood-text');
        if(val > 80) text.innerText = "😡 I am furious!";
        else if(val > 50) text.innerText = "😠 I am still upset.";
        else text.innerText = "💖 I might forgive you...";
    }

    // CHAT
    const messages = [
        { text: "Vaishnavi...", type: "sent", delay: 500 },
        { text: "Please bas poora page end tak padh lo.", type: "sent", delay: 2000 },
        { text: "Uske baad decision tumhara hai.", type: "sent", delay: 4000 }
    ];
    function startChat() {
        const chatBox = document.getElementById('chat-box');
        let index = 0;
        function addMessage() {
            if (index < messages.length) {
                const msgData = messages[index];
                const msgDiv = document.createElement('div');
                msgDiv.className = `msg ${msgData.type}`;
                msgDiv.innerHTML = `${msgData.text}`;
                chatBox.appendChild(msgDiv);
                setTimeout(() => msgDiv.classList.add('show'), 100);
                chatBox.scrollTop = chatBox.scrollHeight;
                index++;
                if (index < messages.length) setTimeout(addMessage, msgData.delay);
                else setTimeout(() => document.getElementById('wa-btn').style.display = 'block', 2000);
            }
        }
        addMessage();
    }

    // PROMISES
    const promises = [
        "I promise to listen more and speak less.",
        "I promise to never take you for granted.",
        "I promise to always bring your favorite Momos.",
        "I promise to focus on fixing problems, not winning arguments.",
        "I promise to never let you feel lonely.",
        "I promise to support your dreams, always."
    ];
    function showPromise() {
        const display = document.getElementById('promise-display');
        const randomPromise = promises[Math.floor(Math.random() * promises.length)];
        display.style.display = 'block';
        display.innerText = "✨ " + randomPromise;
        triggerConfetti(5);
    }

    // CONFETTI
    function openCoupon() {
        document.getElementById('coupon').style.display = 'block';
        triggerConfetti(50);
    }
    function triggerConfetti(count) {
        for(let i=0; i<count; i++) {
            let c = document.createElement("div");
            c.className = "confetti";
            c.style.left = Math.random() * 100 + "vw";
            c.style.background = ["#ff0", "#f00", "#0f0", "#00f"][Math.floor(Math.random()*4)];
            c.style.animationDuration = (Math.random() * 2 + 2) + "s";
            document.body.appendChild(c);
            setTimeout(() => c.remove(), 4000);
        }
    }
</script>

</body>
</html>
