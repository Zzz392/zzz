<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>贪吃蛇游戏</title>
    <style>
        canvas {
            display: block;
            margin: 20px auto;
            border: 1px solid #000;
        }
    </style>
</head>
<body>
 <li>
<a href="https://zzz392.github.io/zzz/1.html">
<img alt="1" src="https://p1.ssl.qhimgs1.com/sdr/400__/t016fe23f8ee7eb2d01.jpg" width="40px" height="40px">
<div>不倒啊？！</div>
</a>
</li>
 <audio controls src="https://zzz392.github.io/zzz/%E5%BC%A0%E6%9D%B0%20-%20%E8%BF%99,%E5%B0%B1%E6%98%AF%E7%88%B1.mp3"></audio>
    <canvas id="gameCanvas" width="400" height="400"></canvas>
    <script>
        const canvas = document.getElementById('gameCanvas');
        const ctx = canvas.getContext('2d');
        const box = 20;
        let snake = [{x: 10, y: 10}];
        let food = {x: 15, y: 15};
        let dX = 0, dY = 0;

        function draw() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            snake.forEach(segment => {
                ctx.fillStyle = 'green';
                ctx.fillRect(segment.x * box, segment.y * box, box, box);
            });
            ctx.fillStyle = 'red';
            ctx.fillRect(food.x * box, food.y * box, box, box);
        }

        function update() {
            const head = {x: snake[0].x + dX, y: snake[0].y + dY};
            snake.unshift(head);
            if (head.x === food.x && head.y === food.y) {
                food = {x: Math.floor(Math.random() * (canvas.width / box)), y: Math.floor(Math.random() * (canvas.height / box))};
            } else {
                snake.pop();
            }
            if (head.x < 0 || head.x >= canvas.width / box || head.y < 0 || head.y >= canvas.height / box) {
                alert('游戏结束');
                document.location.reload();
            }
            for (let i = 1; i < snake.length; i++) {
                if (snake[i].x === head.x && snake[i].y === head.y) {
                    alert('游戏结束');
                    document.location.reload();
                }
            }
        }

        document.addEventListener('keydown', (e) => {
            if (e.key === 'ArrowUp' && dY !== 1) {
                dX = 0; dY = -1;
            } else if (e.key === 'ArrowDown' && dY !== -1) {
                dX = 0; dY = 1;
            } else if (e.key === 'ArrowLeft' && dX !== 1) {
                dX = -1; dY = 0;
            } else if (e.key === 'ArrowRight' && dX !== -1) {
                dX = 1; dY = 0;
            }
        });

        function gameLoop() {
            update();
            draw();
            setTimeout(gameLoop, 100);
        }

        gameLoop();
    </script>
</body>
</html>
