<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Divya</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Poppins', sans-serif;
      background: #111;
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }
    .container {
      padding: 50px 20px;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 20px;
      animation: glow 2s infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 10px #ff00ff; }
      to { text-shadow: 0 0 25px #00ffff; }
    }
    .date {
      font-size: 1.5em;
      margin: 20px 0;
      color: #ffcc00;
      font-weight: bold;
    }
    .names span {
      display: block;
      font-size: 2em;
      margin: 10px 0;
      animation: fadeIn 2s ease forwards;
      opacity: 0;
    }
    .names span:nth-child(1){ animation-delay: 1s; }
    .names span:nth-child(2){ animation-delay: 3s; }
    .names span:nth-child(3){ animation-delay: 5s; }@keyframes fadeIn {
  to { opacity: 1; transform: translateY(0); }
  from { opacity: 0; transform: translateY(30px); }
}

.shayari {
  margin-top: 40px;
  font-size: 1.2em;
  line-height: 1.6em;
}
.shayari p {
  opacity: 0;
  animation: fadeIn 2s ease forwards;
}
.shayari p:nth-child(1){ animation-delay: 7s; }
.shayari p:nth-child(2){ animation-delay: 10s; }
.shayari p:nth-child(3){ animation-delay: 13s; }

.toggle-btn {
  margin-top: 40px;
  padding: 10px 20px;
  background: #ff00cc;
  color: white;
  border: none;
  border-radius: 25px;
  font-size: 1em;
  cursor: pointer;
  box-shadow: 0 0 10px #ff00cc;
}

.light {
  background: #fff !important;
  color: #111 !important;
}

  </style>
</head>
<body>
  <div class="container">
    <h1>🎉 Happy Birthday Divya 🎉</h1>
    <div class="date">12 February 2026</div>
    <div class="names">
      <span>Divya ❤️</span>
      <span>Juhu 🌸</span>
      <span>Avya 💫</span>
    </div><div class="shayari">
  <p>🌷 Tere aane se zindagi me rang aa gaye...</p>
  <p>✨ Teri muskaan se dil ke armaan saj gaye...</p>
  <p>🎂 Khuda kare ye din tere liye khaas ban jaye...</p>
</div>

<button class="toggle-btn" onclick="toggleLight()">💡 Light On/Off</button>

  </div>  <script>
    function toggleLight(){
      document.body.classList.toggle('light');
    }

    // Confetti effect
    function createConfetti(){
      const confetti = document.createElement('div');
      confetti.innerText = '🎊';
      confetti.style.position = 'fixed';
      confetti.style.left = Math.random()*100 + 'vw';
      confetti.style.top = '-5vh';
      confetti.style.fontSize = Math.random()*20+20+'px';
      confetti.style.animation = 'fall 5s linear forwards';
      document.body.appendChild(confetti);
      setTimeout(()=>confetti.remove(),5000);
    }

    setInterval(createConfetti,300);
  </script>  <style>
    @keyframes fall {
      to { transform: translateY(110vh); opacity: 0; }
    }
  </style></body>
</html>
