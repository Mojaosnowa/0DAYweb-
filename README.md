<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>0DAY Конкурс</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #0f0f0f;
      color: #00ff88;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
    header {
      background-color: #1a1a1a;
      width: 100%;
      padding: 30px 20px;
      border-bottom: 2px solid #00ff88;
      display: flex;
      justify-content: center;
      align-items: center;
      box-sizing: border-box;
      position: relative;
    }
    .header-buttons {
      position: absolute;
      left: 20px;
      display: flex;
      gap: 10px;
    }
    .header-buttons button,
    .header-buttons a {
      background-color: #00ff88;
      color: #000;
      border: none;
      padding: 8px 16px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
      text-decoration: none;
      transition: background-color 0.3s;
    }
    .header-buttons button:hover,
    .header-buttons a:hover {
      background-color: #00cc6f;
    }
    .header-title {
      font-size: 2em;
      font-weight: bold;
    }
    main {
      max-width: 800px;
      padding: 30px 20px;
    }
    .rules {
      background-color: #1a1a1a;
      border: 1px solid #00ff88;
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    .rules p {
      margin: 10px 0;
      line-height: 1.6;
    }
    a.social {
      display: inline-block;
      margin: 10px;
      padding: 10px 20px;
      background-color: #00ff88;
      color: #000;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      transition: background-color 0.3s;
    }
    a.social:hover {
      background-color: #00cc6f;
    }
    footer {
      padding: 20px;
      font-size: 0.9em;
      color: #888;
    }
    /* Modal styles */
    .modal {
      display: none;
      position: fixed;
      z-index: 1000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0, 0, 0, 0.7);
    }
    .modal-content {
      background-color: #1a1a1a;
      margin: 10% auto;
      padding: 20px;
      border: 1px solid #00ff88;
      border-radius: 10px;
      width: 300px;
      position: relative;
      color: #00ff88;
    }
    .close {
      position: absolute;
      top: 10px;
      right: 15px;
      color: #00ff88;
      font-size: 20px;
      font-weight: bold;
      cursor: pointer;
    }
    .close:hover {
      color: #ff5555;
    }
    /* Кнопка "Тыкни" красная и шире остальных */
    button#specialBtn {
      background-color: #ff4444;
      color: #fff;
      border: none;
      padding: 12px 36px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
      font-size: 1.1em;
      width: 150px; /* на 50% шире остальных (обычные ~100px) */
      margin: 20px auto 40px;
      display: block;
      transition: background-color 0.3s;
    }
    button#specialBtn:hover {
      background-color: #cc3333;
    }
  </style>
</head>
<body>
  <header>
    <div class="header-buttons">
      <button onclick="openModal('Wawe')">Авторы</button>
      <a href="https://t.me/NiceCanel" target="_blank">ТГК</a>
      <button onclick="openModal('Wawe!')">Победители</button>
    </div>
    <div class="header-title">Приветствуем на сайте 0DAY</div>
  </header>
  <main>
    <div class="rules">
      <p>Этот сайт был создан по причине конкурса на лучшем телеграм канале 0DAY.</p>
      <p>В данном ТГК есть много развлекательного контента, куча конкурсов и большой шанс на победу!</p>
      <p>Залетай к ним — ссылка на ТГК ниже!</p>
    </div>
    <div>
      <a class="social" href="https://t.me/+EhRskyqc7AE0MTZi" target="_blank">Telegram</a>
      <a class="social" href="https://www.tiktok.com/@0day.zone" target="_blank">TikTok</a>
      <a class="social" href="https://www.youtube.com/@Grenki52" target="_blank">YouTube</a>
    </div>
    <button id="specialBtn" onclick="openRickroll()">Тыкни</button>
  </main>
  <footer>
    &copy; 2025 0DAY Contest — Все права защищены
  </footer>

  <!-- Modal -->
  <div id="myModal" class="modal">
    <div class="modal-content">
      <span class="close" onclick="closeModal()">&times;</span>
      <p id="modalText"></p>
    </div>
  </div>

  <script>
    function openModal(message) {
      document.getElementById('modalText').textContent = message;
      document.getElementById('myModal').style.display = 'block';
    }

    function closeModal() {
      document.getElementById('myModal').style.display = 'none';
    }

    window.onclick = function(event) {
      const modal = document.getElementById('myModal');
      if (event.target === modal) {
        closeModal();
      }
    }

    function openRickroll() {
      window.open('https://shattereddisk.github.io/rickroll/rickroll.mp4', '_blank');
    }
  </script>
</body>
</html>
