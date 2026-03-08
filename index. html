<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mercury Game</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body { background-color: #1a1a1a; color: white; text-align: center; font-family: sans-serif; padding-top: 50px; }
        .score { font-size: 48px; margin-bottom: 20px; }
        button { background: #0088cc; color: white; border: none; padding: 20px 40px; border-radius: 50%; font-size: 24px; cursor: pointer; box-shadow: 0 5px #005580; }
        button:active { box-shadow: none; transform: translateY(5px); }
    </style>
</head>
<body>
    <div class="score" id="score">0</div>
    <button id="clickBtn">ЖМИ!</button>

    <script>
        let tg = window.Telegram.WebApp;
        let count = 0;
        let scoreElement = document.getElementById('score');
        let btn = document.getElementById('clickBtn');

        tg.expand(); // Раскрыть на весь экран

        btn.onclick = function() {
            count++;
            scoreElement.innerText = count;
            // Вибрация при нажатии (если телефон поддерживает)
            if (tg.HapticFeedback) {
                tg.HapticFeedback.impactOccurred('medium');
            }
        };
    </script>
</body>
</html>
