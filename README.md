# BIPHUB
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Animated Hello with Falling Flowers</title>
<style>
    body {
        background-color: #000;
        color: #fff;
        font-family: Arial, sans-serif;
        overflow: hidden;
    }

    .container {
        position: relative;
        text-align: center;
        font-size: 50px;
        margin-top: 30vh;
    }

    .flower {
        position: absolute;
        color: #f0f;
        animation: fall 5s linear infinite;
    }

    @keyframes fall {
        0% {
            transform: translateY(-100vh);
        }
        100% {
            transform: translateY(100vh);
        }
    }

    .flower:nth-child(1) {
        left: 5%;
        animation-delay: 0s;
    }

    .flower:nth-child(2) {
        left: 25%;
        animation-delay: 1s;
    }

    .flower:nth-child(3) {
        left: 45%;
        animation-delay: 2s;
    }

    .flower:nth-child(4) {
        left: 65%;
        animation-delay: 3s;
    }

    .flower:nth-child(5) {
        left: 85%;
        animation-delay: 4s;
    }
</style>
</head>
<body>
<div class="container">
    <div class="flower">❀</div>
    <div class="flower">❁</div>
    <div class="flower">✿</div>
    <div class="flower">❃</div>
    <div class="flower">❋</div>
</div>
</body>
</html>
