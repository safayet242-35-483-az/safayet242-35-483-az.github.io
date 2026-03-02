# safayet242-35-483-az.github.io<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Azra Adiba! 💕</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-family: 'Georgia', serif;
            overflow: hidden;
        }

        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.95);
            padding: 60px;
            border-radius: 30px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            max-width: 700px;
            animation: slideIn 0.8s ease-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            background: linear-gradient(45deg, #ff69b4, #ff1493, #ffb6c1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-size: 2.5em;
            margin-bottom: 30px;
            animation: bounce 1s ease-in-out infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .cake-btn {
            font-size: 120px;
            cursor: pointer;
            transition: transform 0.3s, filter 0.3s;
            margin: 30px 0;
            display: inline-block;
        }

        .cake-btn:hover {
            transform: scale(1.15);
            filter: drop-shadow(0 0 20px rgba(255, 105, 180, 0.8));
        }

        .cake-btn:active {
            transform: scale(0.95);
        }

        .message {
            font-size: 28px;
            font-weight: bold;
            margin: 20px 0;
            min-height: 60px;
            opacity: 0;
            animation: fadeInUp 1s ease-out forwards;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .msg1 {
            color: #ff69b4;
            font-style: italic;
        }

        .msg2 {
            color: #ff1493;
            font-weight: 900;
        }

        .msg3 {
            color: #c71585;
        }

        .note {
            margin-top: 50px;
            padding: 30px;
            background: linear-gradient(135deg, #ffe5ec 0%, #fff0f5 100%);
            border-left: 5px solid #ff69b4;
            border-radius: 10px;
            font-size: 18px;
            color: #333;
            font-style: italic;
            line-height: 1.8;
        }

        .confetti {
            position: fixed;
            width: 10px;
            height: 10px;
            opacity: 0.8;
            animation: fall linear infinite;
        }

        @keyframes fall {
            to {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }

        .click-text {
            color: #999;
            font-size: 14px;
            margin-top: 20px;
        }

        .balloon {
            position: fixed;
            width: 30px;
            height: 40px;
            border-radius: 50% 50% 50% 0;
            opacity: 0.7;
            animation: float 4s ease-in-out infinite;
        }

        .balloon1 { left: 5%; background: #ff6b6b; animation-delay: 0s; }
        .balloon2 { left: 15%; background: #4ecdc4; animation-delay: 1s; }
        .balloon3 { right: 15%; background: #ffe66d; animation-delay: 2s; }
        .balloon4 { right: 5%; background: #ff69b4; animation-delay: 3s; }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-40px); }
        }
    </style>
</head>
<body>
    <div class="balloon balloon1"></div>
    <div class="balloon balloon2"></div>
    <div class="balloon balloon3"></div>
    <div class="balloon balloon4"></div>

    <div class="container">
        <h1>✨ Happy Birthday Azra Adiba ✨</h1>
        
        <p class="click-text">Click the cake below! 🎂</p>
        
        <div class="cake-btn" onclick="revealMessages()">🎂</div>

        <div id="message1" class="message msg1" style="display:none;">Happy Birthday to my mayabi! 💕</div>
        <div id="message2" class="message msg2" style="display:none;">pakhi adib 🐦</div>
        <div id="message3" class="message msg3" style="display:none;">Happy Birthday to you Adiba! 🎉</div>

        <div class="note">
            "Be my march not loud like summer,<br>Just warm enough to bring me back to life" 🌸❄️
        </div>
    </div>

    <script>
        function revealMessages() {
            const msg1 = document.getElementById('message1');
            const msg2 = document.getElementById('message2');
            const msg3 = document.getElementById('message3');

            msg1.style.display = 'block';
            msg1.style.animationDelay = '0s';

            setTimeout(() => {
                msg2.style.display = 'block';
                msg2.style.animationDelay = '0s';
            }, 1000);

            setTimeout(() => {
                msg3.style.display = 'block';
                msg3.style.animationDelay = '0s';
            }, 2000);

            createConfetti();
        }

        function createConfetti() {
            for (let i = 0; i < 40; i++) {
                const confetti = document.createElement('div');
                confetti.className = 'confetti';
                confetti.style.left = Math.random() * 100 + '%';
                confetti.style.backgroundColor = ['#ff6b6b', '#4ecdc4', '#ffe66d', '#ff69b4', '#ffb6c1'][Math.floor(Math.random() * 5)];
                confetti.style.animationDuration = (2 + Math.random() * 2) + 's';
                document.body.appendChild(confetti);

                setTimeout(() => confetti.remove(), 4000);
            }
        }
    </script>
</body>
</html>