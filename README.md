# YO-MAARTEN.nl
<!DOCTYPE html>
<html lang="nl">
<head>
  <meta charset="UTF-8">
  <title>YO MAARTEN</title>
  <style>
    body {
      margin: 0;
      background-color: #111;
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      font-family: Arial, sans-serif;
    }

    .stickman {
      position: relative;
      animation: wave 1s infinite alternate;
    }

    .head {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      border: 3px solid white;
      margin: 0 auto;
    }

    .body {
      width: 3px;
      height: 80px;
      background: white;
      margin: 0 auto;
    }

    .arms {
      width: 60px;
      height: 3px;
      background: white;
      margin: 0 auto;
    }

    .legs {
      display: flex;
      justify-content: space-between;
      width: 40px;
      margin: 0 auto;
    }

    .legs div {
      width: 3px;
      height: 60px;
      background: white;
    }

    @keyframes wave {
      0% { transform: rotate(-5deg); }
      100% { transform: rotate(5deg); }
    }
  </style>
</head>
<body>
  <div class="stickman">
    <div class="head"></div>
    <div class="arms"></div>
    <div class="body"></div>
    <div class="legs">
      <div></div>
      <div></div>
    </div>
  </div>

  <audio autoplay>
    <source src="yo-maarten.mp3" type="audio/mpeg">
    Je browser ondersteunt geen audio :(
  </audio>
</body>
</html>
<!DOCTYPE html>
<html lang="nl">
<head>
  <meta charset="UTF-8">
  <title>YO MAARTEN</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>YO MAARTEN</h1>
  <div class="stickman">
    <div class="head"></div>
    <div class="body"></div>
    <div class="arms"></div>
    <div class="legs"></div>
  </div>
  <button onclick="playSound()">Laat hem roepen!</button>

  <audio id="yoAudio" src="yo-maarten.mp3"></audio>

  <script>
    function playSound() {
      document.getElementById("yoAudio").play();
    }
  </script>
</body>
</html>
body {
  text-align: center;
  font-family: Arial, sans-serif;
  background: linear-gradient(to bottom, #111, #333);
  color: white;
  padding-top: 50px;
}

h1 {
  font-size: 3em;
  margin-bottom: 20px;
}

.stickman {
  margin: 20px auto;
  width: 20px;
  animation: bounce 1s infinite alternate;
}

.head {
  width: 20px;
  height: 20px;
  border: 2px solid white;
  border-radius: 50%;
  margin: 0 auto;
}

.body {
  width: 2px;
  height: 40px;
  background: white;
  margin: 0 auto;
}

.arms {
  width: 40px;
  height: 2px;
  background: white;
  margin: -1px auto;
}

.legs {
  width: 2px;
  height: 30px;
  background: white;
  margin: 2px auto;
  transform: rotate(20deg);
}

@keyframes bounce {
  0% { transform: translateY(0px); }
  100% { transform: translateY(-20px); }
}

button {
  margin-top: 30px;
  padding: 10px 20px;
  font-size: 1.2em;
  cursor: pointer;
  background: #ff0055;
  border: none;
  color: white;
  border-radius: 10px;
}
