<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <title>Kattintás Játék</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
        }
        .game {
            text-align: center;
        }
        #score {
            font-size: 2em;
            margin-bottom: 20px;
        }
        #clickButton {
            padding: 10px 20px;
            font-size: 1.5em;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="game">
        <div id="score">Pontok: 0</div>
        <button id="clickButton">Kattints Rám!</button>
    </div>

    <script>
        let score = 0;
        const scoreDisplay = document.getElementById('score');
        const clickButton = document.getElementById('clickButton');

        clickButton.addEventListener('click', () => {
            score++;
            scoreDisplay.textContent = `Pontok: ${score}`;
        });
    </script>
</body>
</html>
