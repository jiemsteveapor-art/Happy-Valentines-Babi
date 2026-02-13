<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Normelen ❤️</title>
<style>
    body {
        margin: 0;
        font-family: 'Segoe UI', sans-serif;
        background: linear-gradient(to bottom right, #ff9a9e, #fad0c4);
        overflow: hidden;
        text-align: center;
    }

    /* Background hearts */
    .heart {
        position: absolute;
        color: rgba(255, 255, 255, 0.7);
        font-size: 20px;
        animation: float 10s linear infinite;
    }

    @keyframes float {
        from { transform: translateY(100vh); }
        to { transform: translateY(-10vh); }
    }

    /* Popup */
    .popup {
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        background: white;
        width: 85%;
        max-width: 500px;
        padding: 30px;
        border-radius: 20px;
        box-shadow: 0 15px 40px rgba(0,0,0,0.3);
        text-align: center;
        animation: fadeIn 1.5s ease-in-out;
        z-index: 10;
    }

    @keyframes fadeIn {
        from { opacity: 0; transform: translate(-50%, -60%); }
        to { opacity: 1; transform: translate(-50%, -50%); }
    }

    .popup h2 {
        margin-top: 0;
        color: #ff4e78;
    }

    .popup p {
        color: #444;
        line-height: 1.6;
        font-size: 1em;
    }

    .popup button {
        margin-top: 20px;
        padding: 10px 25px;
        border: none;
        border-radius: 25px;
        background-color: #ff4e78;
        color: white;
        cursor: pointer;
        transition: 0.3s;
    }

    .popup button:hover {
        background-color: #ff1e56;
        transform: scale(1.1);
    }

    /* Main Content */
    .main {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        display: none;
    }

    .sunflower {
        font-size: 80px;
        margin-bottom: 20px;
    }

</style>
</head>
<body>

<!-- Love Letter Popup -->
<div class="popup" id="lovePopup">
    <h2>💌 A Letter For You, Normelen 💌</h2>
    <p>
        My beautiful Normelen,<br><br>
        It has been 2 amazing years together, and I still can’t believe how far we have come. 
        From our first conversations to all the memories we’ve created, every moment with you 
        has meant the world to me.<br><br>

        We have grown, learned, laughed, and loved through everything. 
        These two years have shown me how strong our bond is and how real our love is.<br><br>

        You are my happiness, my peace, and my sunshine — just like the sunflowers you love. 🌻<br><br>

        Thank you for choosing me every day. 
        I can’t wait for all the years ahead of us.<br><br>

        Happy Valentine’s Day, my love ❤️
    </p>
    <button onclick="closePopup()">Open Your Surprise 🌻</button>
</div>

<!-- Main Surprise Content -->
<div class="main" id="mainContent">
    <div class="sunflower">🌻</div>
    <h1 style="font-size: 3em;">Happy Valentine's Day, Normelen ❤️</h1>
    <p style="font-size: 1.3em;">
        You are the best thing that has ever happened to me.  
        I love you more than words can explain. 🌻
    </p>
</div>

<script>
    function closePopup() {
        document.getElementById("lovePopup").style.display = "none";
        document.getElementById("mainContent").style.display = "block";
    }

    // Floating hearts generator
    for (let i = 0; i < 25; i++) {
        let heart = document.createElement("div");
        heart.classList.add("heart");
        heart.innerHTML = "❤️";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = (5 + Math.random() * 5) + "s";
        heart.style.fontSize = (15 + Math.random() * 25) + "px";
        document.body.appendChild(heart);
    }
</script>

</body>
</html>
# Happy-Valentines-Babi
