mi-pagina-juegos/  ← raíz
   └── index.html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi Mega Página de Juegos</title>
  <style>
    body {
      background: #1a1a1a;
      color: white;
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 0;
      padding: 0;
    }
    header {
      background: #333;
      padding: 15px;
    }
    h1 {
      margin: 0;
    }
    nav {
      margin: 20px 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
    }
    button {
      background: #555;
      color: white;
      border: none;
      padding: 8px 15px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 14px;
    }
    button:hover {
      background: #777;
    }
    iframe {
      border: 3px solid #444;
      border-radius: 10px;
      width: 800px;
      height: 500px;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>🎮 Mi Mega Página de Juegos 🎮</h1>
  </header>

  <nav id="gameButtons">
    <!-- Botones se agregan desde JS -->
  </nav>

  <iframe id="gameFrame" src=""></iframe>

  <script>
    // Lista de juegos: [nombre, URL]
    const juegos = [
      ["Snake", "https://playsnake.org/"],
      ["Tetris", "https://tetris.com/play-tetris"],
      ["Pac-Man", "https://pacman.live/"],
      ["Flappy Bird", "https://flappybird.io/"],
      ["2048", "https://play2048.co/"],
      ["Mario", "https://supermarioemulator.com/mario.php"],
      ["Solitaire", "https://www.solitr.com/"],
      ["Minesweeper", "https://minesweeper.online/"],
      ["Chrome Dino", "https://chromedino.com/"],
      ["Basketball", "https://www.crazygames.com/game/basketball-heroes"],
      // Agregar más hasta 50...
    ];

    // Generar botones dinámicamente
    const nav = document.getElementById("gameButtons");
    juegos.forEach(j => {
      const btn = document.createElement("button");
      btn.innerText = j[0];
      btn.onclick = () => {
        document.getElementById("gameFrame").src = j[1];
      };
      nav.appendChild(btn);
    });

    // Botón especial para Roblox
    const robloxBtn = document.createElement("button");
    robloxBtn.innerText = "Roblox";
    robloxBtn.onclick = () => {
      window.open("https://www.roblox.com/games", "_blank");
    };
    nav.appendChild(robloxBtn);
  </script>
</body>
</html>
