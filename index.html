<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Padel Tournament Scorekeeper</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f7f7f7;
      color: #111;
      padding: 16px;
    }

    .container {
      max-width: 480px;
      margin: 0 auto;
      background: #fff;
      border-radius: 16px;
      padding: 20px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.08);
    }

    h1 {
      font-size: 22px;
      margin-bottom: 20px;
      text-align: center;
    }

    h2 {
      font-size: 18px;
      margin: 20px 0 10px;
    }

    label {
      display: block;
      font-size: 14px;
      margin-bottom: 6px;
      font-weight: 600;
    }

    input, select, button {
      width: 100%;
      padding: 12px;
      border: 1px solid #ddd;
      border-radius: 10px;
      font-size: 16px;
      margin-bottom: 12px;
    }

    button {
      background: #111;
      color: white;
      border: none;
      font-weight: 700;
      cursor: pointer;
    }

    .pair {
      background: #fafafa;
      border: 1px solid #eee;
      border-radius: 12px;
      padding: 14px;
      margin-bottom: 14px;
    }

    .score-box {
      font-size: 18px;
      font-weight: bold;
      text-align: center;
      margin-top: 8px;
    }

    .muted {
      font-size: 13px;
      color: #666;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Padel Tournament</h1>

    <h2>Настройки</h2>

    <label>Количество участников</label>
    <select id="playersCount">
      <option value="4">4</option>
      <option value="8">8</option>
      <option value="12">12</option>
      <option value="16">16</option>
    </select>

    <label>Игра до (сумма очков)</label>
    <input type="number" id="maxPoints" value="19" min="1" />

    <button onclick="generatePlayers()">Создать участников</button>

    <div id="playersArea"></div>

    <button onclick="generatePairs()">Сформировать пары</button>

    <div id="pairsArea"></div>
  </div>

  <script>
    let players = [];

    function generatePlayers() {
      const count = parseInt(document.getElementById('playersCount').value);
      const area = document.getElementById('playersArea');
      area.innerHTML = '<h2>Имена участников</h2>';

      for (let i = 1; i <= count; i++) {
        area.innerHTML += `
          <label>Игрок ${i}</label>
          <input type="text" id="player${i}" placeholder="Имя игрока ${i}" value="Игрок ${i}" />
        `;
      }
    }

    function shuffle(array) {
      for (let i = array.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [array[i], array[j]] = [array[j], array[i]];
      }
      return array;
    }

    function generatePairs() {
      const count = parseInt(document.getElementById('playersCount').value);
      const maxPoints = parseInt(document.getElementById('maxPoints').value);

      players = [];
      for (let i = 1; i <= count; i++) {
        players.push(document.getElementById(`player${i}`).value || `Игрок ${i}`);
      }

      shuffle(players);

      const area = document.getElementById('pairsArea');
      area.innerHTML = '<h2>Матчи</h2>';

      for (let i = 0; i < players.length; i += 4) {
        if (!players[i + 3]) break;

        const team1 = `${players[i]} / ${players[i + 1]}`;
        const team2 = `${players[i + 2]} / ${players[i + 3]}`;

        area.innerHTML += `
          <div class="pair">
            <div><strong>Пара 1:</strong> ${team1}</div>
            <div><strong>Пара 2:</strong> ${team2}</div>

            <label>Очки пары 1</label>
            <input
              type="number"
              min="0"
              max="${maxPoints}"
              value="0"
              oninput="updateScore(this, ${maxPoints})"
            />

            <div class="score-box">
              Пара 2: <span>0</span>
            </div>

            <div class="muted">Очки второй пары считаются автоматически</div>
          </div>
        `;
      }
    }

    function updateScore(input, maxPoints) {
      let first = parseInt(input.value) || 0;

      if (first > maxPoints) {
        first = maxPoints;
        input.value = maxPoints;
      }

      const second = Math.max(0, maxPoints - first);
      input.parentElement.querySelector('span').textContent = second;
    }
  </script>
</body>
</html>
