
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rainer</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      transition: background-color 1s ease;
    }

    img {
      max-width: 80%;
      max-height: 60%;
      border-radius: 12px;
      box-shadow: 0px 0px 20px rgba(0,0,0,0.4);
    }

    button {
      margin-top: 20px;
      padding: 12px 24px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      background: #333;
      color: white;
      box-shadow: 0px 4px 10px rgba(0,0,0,0.3);
      transition: background 0.3s;
    }

    button:hover {
      background: #555;
    }
  </style>
</head>
<body>
  <!-- Dein eigenes Bild -->
  <img src="dein-bild.png" alt="Mein Bild">

  <!-- Audio Button -->
  <button onclick="playAudio()">Audio</button>

  <!-- Audio Datei -->
  <audio id="myAudio" src="musik.mp3"></audio>

  <script>
    // Hintergrundfarben
    const colors = ["#ff9999", "#99ccff", "#99ff99", "#ffff99", "#ffcc99", "#cc99ff"];
    let i = 0;

    setInterval(() => {
      document.body.style.backgroundColor = colors[i];
      i = (i + 1) % colors.length;
    }, 2000);

    // Audio abspielen
    function playAudio() {
      const audio = document.getElementById("myAudio");
      audio.play();
    }
  </script>
</body>
</html>
