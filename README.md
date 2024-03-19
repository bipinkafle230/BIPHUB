# BIPHUB
My time pass>>>>>>>>>>>>>
<!DOCTYPE html>
<html lang="en">
<head>
 <script >
 function playMusic() {
      document.getElementById('musicPlayer').play();
 }

 function pauseMusic() {
      document.getElementById('musicPlayer').pause();
 }

 function stopMusic() {
      var musicPlayer = document.getElementById('musicPlayer');
      musicPlayer.pause();
      musicPlayer.currentTime = 0;
 }

 window.onload = function() {
    document.getElementById('musicPlayer').play();
 }
 </script>
    <style>
        body {
            color: black;
            font-size: 20px;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            text-align: center;
            text-decoration: underline;
            text-transform: capitalize;
            text-shadow: 10px 10px 10px red;
            line-height: 20px;
            
            background-image: url("c:\Users\DELL\Downloads\siblings-817369_1280.jpg");
            background-size: cover;
            background-repeat: no-repeat;
            animation: colorChange 10s infinite, vibrate 1s infinite;
        }
        @keyframes colorChange {
            0% {
                background-color: aqua;
                color: rgb(236, 18, 210);
            }
            25% {
                background-color: rgb(255, 221, 0);
                color: rgb(33, 26, 111);
            }
            50% {
                background-color: rgb(42, 154, 191);
                color: rgb(175, 36, 36);
            }
            100% {
                background-color: rgb(227, 17, 17);
                color: rgb(211, 41, 41);
            }
        }
   

        @keyframes vibrate {
            0%, 100% {
                transform: translate(0);
            }
            10%, 30%, 50%, 70%, 90% {
                transform: translate(10px);
            }
            20%, 40%, 60%, 80% {
                transform: translate(-10px);
            }
        }

        .button-toplay {
            text-align: center;
            font-size: 30px;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            text-transform: capitalize;
            text-shadow: 10px 10px 10px red;
            line-height: 20px;
        }
    </style>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <canvas id="canvas" width="500" height="500">
        <p>your browser does not support canvas</p>
        <script src="Zkh.js"></script>         
    </canvas>
    <audio id="musicPlayer">
        <source src="c:\Users\DELL\Downloads\Tu he na ..............mp3" type="audio/mp3">
    </audio>
    <div class="button-toplay">
        <button onclick="playMusic()">Play</button>
        <button onclick="pauseMusic()">Pause</button>
        <button onclick="stopMusic()">Stop</button>
        <!-- Add other buttons as needed -->
    </div>
    <svg width="500" height="500">
        <!-- Draw lines for the staff -->
        <line x1="50" y1="100" x2="450" y2="100" style="stroke:rgb(0,0,0);stroke-width:2" />
        <line x1="50" y1="150" x2="450" y2="150" style="stroke:rgb(0,0,0);stroke-width:2" />
        <line x1="50" y1="200" x2="450" y2="200" style="stroke:rgb(0,0,0);stroke-width:2" />
        <line x1="50" y1="250" x2="450" y2="250" style="stroke:rgb(0,0,0);stroke-width:2" />
        <line x1="50" y1="300" x2="450" y2="300" style="stroke:rgb(0,0,0);stroke-width:2" />
        <!-- Add notes as needed -->
    </svg>
</body>
</html>
