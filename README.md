
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
      justify-content: center;
      align-items: center;
      transition: background-color 1s ease;
    }

    img {
      max-width: 80%;
      max-height: 80%;
      border-radius: 12px;
      box-shadow: 0px 0px 20px rgba(0,0,0,0.4);
    }
  </style>
</head>
<body>
  <!-- Dein eigenes Bild einfügen -->
  <img src="dein-bild.png" alt="Mein Bild">

  <script>
    const colors = ["#ff9999", "#99ccff", "#99ff99", "#ffff99", "#ffcc99", "#cc99ff"];
    let i = 0;

    setInterval(() => {
      document.body.style.backgroundColor = colors[i];
      i = (i + 1) % colors.length;
    }, 2000);
  </script>
</body>
</html>
