# WED
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi Página de Juegos</title>
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
    .game-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin: 30px;
    }
    iframe {
      border: 3px solid #444;
      border-radius: 10px;
      width: 400px;
      height: 400px;
    }
  </style>
</head>
<body>
  <header>
    <h1>🎮 Mi Página de Juegos 🎮</h1>
  </header>
  
  <div class="game-container">
    <!-- Snake -->
    <iframe src="https://playsnake.org/"></iframe>

    <!-- Tetris -->
    <iframe src="https://tetris.com/play-tetris"></iframe>

    <!-- Pac-Man -->
    <iframe src="https://pacman.live/"></iframe>

    <!-- Flappy Bird -->
    <iframe src="https://flappybird.io/"></iframe>

    <!-- 2048 -->
    <iframe src="https://play2048.co/"></iframe>

    <!-- Mario Remake -->
    <iframe src="https://supermarioemulator.com/mario.php"></iframe>
  </div>
</body>
</html>
