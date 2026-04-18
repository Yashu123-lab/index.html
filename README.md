# index.html
<!DOCTYPE html>
<html>
<head>
  <title>My First Website</title>
</head>
<body>
  <h1>Hello 👋 My Website is Live!</h1>
  <p>Built using GitHub Pages</p>
</body>
</html>
<!DOCTYPE html>
<html>
  <div class="card">
    <h3>📊 Smart Support & Resistance (Auto Detection)</h3>

    <textarea id="priceData" placeholder="Enter prices like: 100,102,98,105,97,100,101,98"></textarea><br><br>

    <button onclick="smartSR()">Generate Smart Levels</button>

    <canvas id="chart" width="350" height="200" style="background:#111; border-radius:10px;"></canvas>

    <p id="srResult"></p>
</div>
  <div class="card">
    <h3>📊 Auto Support & Resistance</h3>

    <textarea id="priceData" placeholder="Enter prices (comma separated) e.g. 100,102,98,105,97"></textarea><br><br>

    <button onclick="drawLevels()">Draw Levels</button>

    <canvas id="chart" width="350" height="200" style="background:#111; border-radius:10px;"></canvas>
</div>
  
  <div class="card">
    <h3>🧪 Test Strategy</h3>

    <input type="number" id="price" placeholder="Current Price"><br><br>
    <input type="number" id="support" placeholder="Support"><br><br>
    <input type="number" id="resistance" placeholder="Resistance"><br><br>

    <button onclick="runStrategy()">Check Signal</button>

    <p id="signalResult"></p>
    
</div>
  <div class="card" onclick="toggle('realStrategy')">
    <h3>🔥 Real Strategy: Support + Candle</h3>

    <div id="realStrategy" class="content">
        Step 1: Mark Support Zone<br>
        Step 2: Wait for price to touch support<br>
        Step 3: Look for Hammer candle 🕯️<br><br>

        👉 Entry: After candle close<br>
        👉 Stop Loss: Below wick<br>
        👉 Target: Next resistance<br><br>

        ✔ High probability setup
    </div>
</div>
  <div class="card">
    <h3>📊 Live Market Chart</h3>

    <iframe 
        src="https://s.tradingview.com/widgetembed/?symbol=BINANCE:BTCUSDT&interval=1&theme=dark"
        style="width:100%; height:400px; border:none;">
    </iframe>
</div>
  <button onclick="showTips()">Show Trading Tip</button>
<p id="tip" style="display:none;">👉 Always use Stop Loss!</p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Retail_store.jpg/320px-Retail_store.jpg">
  <div class="card" onclick="toggle('retail')">
    <h3>🛒 Retailing (Full Explanation)</h3>
    <div id="retail" class="content">

        <b>📌 Definition:</b><br>
        Retailing means selling goods directly to final consumers for personal use.<br><br>

        <b>📦 Example:</b><br>
        Buying clothes, food, mobile → all are retail.<br><br>

        <b>🔄 Retail vs Wholesale:</b><br>
        Retail = sells to customer (small quantity)<br>
        Wholesale = sells to shop (large quantity)<br><br>

        <b>🏪 Types of Retailing:</b><br>
        1. Store Retailing → Shop, mall<br>
        2. Non-store → Online, door-to-door<br><br>

        <b>⚙️ Functions of Retailer:</b><br>
        - Buy goods<br>
        - Store goods<br>
        - Sell in small quantity<br>
        - Help customers<br><br>

        <b>⭐ Importance:</b><br>
        - Easy availability<br>
        - Saves time<br>
        - Provides variety<br><br>

        <b>🔁 Flow:</b><br>
        Manufacturer → Wholesaler → Retailer → Customer

    </div>
</div>
  <input type="number" id="slPrice" placeholder="Stop Loss Price"><br><br>
<input type="number" id="targetPrice" placeholder="Target Price"><br><br>
<head>
    <title>Yash Trading Pro</title>
    container{
    <div class="card" onclick="toggle('str1')">
    <h3>📈 Strategy 1: Trend + Support</h3>
    <div id="str1" class="content">
        Step 1: Identify Uptrend (Higher High + Higher Low)<br>
        Step 2: Mark Support Zone<br>
        Step 3: Wait for price to come near support<br>
        Step 4: Enter Buy<br><br>

        👉 Stop Loss: Below support<br>
        👉 Target: Next resistance<br><br>

        ✔ Works best in trending market
    </div>
</div>

<div class="card" onclick="toggle('str2')">
    <h3>🕯️ Strategy 2: Candle Reversal</h3>
    <div id="str2" class="content">
        Step 1: Find Support or Resistance<br>
        Step 2: Wait for reversal candle<br><br>

        👉 Buy signal:
        - Hammer at support<br>

        👉 Sell signal:
        - Shooting star at resistance<br><br>

        👉 Stop Loss:
        - Below/Above candle wick<br><br>

        ✔ Good for quick entries
    </div>
</div>

<div class="card" onclick="toggle('str3')">
    <h3>⚡ Strategy 3: EMA Trend Strategy</h3>
    <div id="str3" class="content">
        Step 1: Add EMA (50)<br>
        Step 2: Check trend<br><br>

        👉 Buy:
        - Price above EMA<br>
        - Pullback to EMA<br>

        👉 Sell:
        - Price below EMA<br>
        - Pullback to EMA<br><br>

        👉 Stop Loss:
        - Below/Above EMA<br><br>

        ✔ Simple and powerful strategy
    </div>
</div>

    <style>
    body {
    font-family: 'Segoe UI', Arial;
    margin: 0;
    background: #0b1220;
    color: white;
}

/* Header */
header {
    background: #020617;
    padding: 18px;
    text-align: center;
    font-size: 24px;
    font-weight: bold;
    letter-spacing: 1px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.5);
}

/* Container */
.container {
    padding: 20px;
    <div class="card">
    <h3>🤖 Advanced Signal Generator</h3>

    <input type="number" id="price" placeholder="Current Price"><br><br>
    <input type="number" id="ema" placeholder="EMA (Trend Line)"><br><br>
    <input type="number" id="support" placeholder="Support"><br><br>
    <input type="number" id="resistance" placeholder="Resistance"><br><br>
    <input type="number" id="sl" placeholder="Stop Loss"><br><br>
    <input type="number" id="target" placeholder="Target"><br><br>

    <button onclick="generateSignal()">Generate Signal</button>

    <h4 id="signalOutput"></h4>
</div
}

/* Cards */
.card {
    background: #111827;
    padding: 18px;
    margin: 15px 0;
    border-radius: 14px;
    cursor: pointer;
    transition: 0.3s;
    box-shadow: 0 0 10px rgba(0,0,0,0.4);
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 0 20px rgba(34,197,94,0.3);
}

/* Content */
.content {<div class="card">
    <h3>🤖 Advanced Signal Generator</h3>

    <input type="number" id="price" placeholder="Current Price"><br><br>
    <input type="number" id="ema" placeholder="EMA (Trend Line)"><br><br>
    <input type="number" id="support" placeholder="Support"><br><br>
    <input type="number" id="resistance" placeholder="Resistance"><br><br>
    <input type="number" id="sl" placeholder="Stop Loss"><br><br>
    <input type="number" id="target" placeholder="Target"><br><br>

    <button onclick="generateSignal()">Generate Signal</button>

    <h4 id="signalOutput"></h4>
</div>
    display: none;
    margin-top: 10px;
    color: #9ca3af;
    line-height: 1.6;
}

/* Inputs */
input {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border-radius: 8px;
    border: none;
    outline: none;
}

/* Buttons */
button {
    padding: 10px 15px;
    margin-top: 10px;
    background: linear-gradient(45deg, #22c55e, #4ade80);
    border: none;
    border-radius: 8px;
    cursor: pointer;
    color: black;
    font-weight: bold;
    transition: 0.3s;
}

button:hover {
    transform: scale(1.05);
}

/* Trade List */
ul {
    list-style: none;
    padding: 0;
}

li {
    background: #1f2933;
    margin: 8px 0;
    padding: 10px;
    border-radius: 8px;
    font-size: 14px;
}

        header {
          <header>📊 Yash Trading Pro</header>
            background: #020617;
            padding: 15px;
            text-align: center;
            font-size: 22px;
            font-weight: bold;
        }

        .container
        {<h2 style="text-align:center; margin-bottom:20px;">Learn • Practice • Grow</h2>
            padding: 20px;
        }

        .card {
            background: #1e293b;
            padding: 15px;
            margin: 12px 0;
            border-radius: 10px;
            cursor: pointer;
        }

        .card:hover {
            background: #334155;
        }

        .content {
            display: none;
            margin-top: 10px;
            color: #cbd5f5;
        }

        img {
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }

        button {
            margin: 5px;
            padding: 8px 12px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }
    </style>
</head>

<body>

<header>📊 Yash Trading Pro Learning</header>

<div class="container">

<!-- BASIC -->
<div class="card" onclick="toggle('basic')">
    <h3>📚 Basics</h3>
    <div id="basic" class="content">
        Support = price stops falling 📉<br>
        Resistance = price stops rising 📈<br><br>

        Uptrend = Higher High + Higher Low<br>
        Downtrend = Lower High + Lower Low<br><br>

        Always follow trend ✔
    </div>
</div>

<!-- CANDLE -->
<div class="card" onclick="toggle('candle')">
    <h3>🕯️ Candlestick Patterns</h3>
    <div id="candle" class="content">

        <b>Hammer 🔨</b><br>
        Strong rejection from bottom → Buy signal<br>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Candlestick_bullish_hammer.png/320px-Candlestick_bullish_hammer.png">

        <br><br>

        <b>Shooting Star ⭐</b><br>
        Rejection from top → Sell signal<br>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7f/Candlestick_bearish_shooting_star.png/320px-Candlestick_bearish_shooting_star.png">

    </div>
</div>

<!-- STRATEGY -->
<div class="card" onclick="toggle('strategy')">
    <h3>📈 Simple Strategy</h3>
    <div id="strategy" class="content">

        Step 1: Find Trend<br>
        Step 2: Mark Support/Resistance<br>
        Step 3: Wait for Candle Pattern<br><br>

        👉 Buy Setup:
        - Uptrend
        - Price near support
        - Hammer candle

        <br><br>

        👉 Sell Setup:
        - Downtrend
        - Price near resistance
        - Shooting star

    </div>
</div>

<!-- QUIZ -->
<div class="card">
    <h3>🧠 Quiz</h3>

  <div class="card">
    <h3>🧠 Trading Quiz</h3>

    <div id="quizBox"></div>

    <button onclick="submitQuiz()">Submit Quiz</button>

    <h4 id="scoreResult"></h4>
</div>
</div>

</div>
container
<div class="card">
    <h3>🧠 AI Signal System</h3>

    <input type="number" id="priceAI" placeholder="Current Price"><br><br>
    <input type="number" id="emaAI" placeholder="EMA"><br><br>
    <input type="number" id="supportAI" placeholder="Support"><br><br>
    <input type="number" id="resistanceAI" placeholder="Resistance"><br><br>
    <input type="number" id="slAI" placeholder="Stop Loss"><br><br>
    <input type="number" id="targetAI" placeholder="Target"><br><br>

    <button onclick="aiSignal()">Generate AI Signal</button>

    <h4 id="aiResult"></h4>
</div>

<script>
  function goldZones() {
    let data = document.getElementById("goldData").value;
    let prices = data.split(",").map(Number);

    let canvas = document.getElementById("goldChart");
    let ctx = canvas.getContext("2d");

    ctx.clearRect(0, 0, canvas.width, canvas.height);

    let max = Math.max(...prices);
    let min = Math.min(...prices);

    // -------------------------
    // DRAW PRICE LINE
    // -------------------------
    ctx.beginPath();
    prices.forEach((p, i) => {
        let x = (i / (prices.length - 1)) * canvas.width;
        let y = canvas.height - ((p - min) / (max - min)) * canvas.height;

        if (i === 0) ctx.moveTo(x, y);
        else ctx.lineTo(x, y);
    });
    ctx.strokeStyle = "white";
    ctx.stroke();

    // -------------------------
    // SMART ZONES (SUPPORT/RESISTANCE)
    // -------------------------
    let tolerance = (max - min) * 0.02;
    let zones = [];

    prices.forEach(p => {
        let found = false;

        for (let z of zones) {
            if (Math.abs(z.price - p) <= tolerance) {
                z.price = (z.price + p) / 2;
                z.count++;
                found = true;
                break;
            }
        }

        if (!found) {
            zones.push({ price: p, count: 1 });
        }
    });

    let strongZones = zones.filter(z => z.count >= 2);

    // -------------------------
    // DRAW ZONES
    // -------------------------
    strongZones.forEach(z => {
        let y = canvas.height - ((z.price - min) / (max - min)) * canvas.height;

        ctx.beginPath();
        ctx.moveTo(0, y);
        ctx.lineTo(canvas.width, y);

        ctx.strokeStyle = "#22c55e";
        ctx.lineWidth = 2;
        ctx.stroke();
    });

    // -------------------------
    // BUY / SELL LOGIC
    // -------------------------
    let lastPrice = prices[prices.length - 1];

    let support = Math.min(...strongZones.map(z => z.price));
    let resistance = Math.max(...strongZones.map(z => z.price));

    let signal = "";

    if (lastPrice <= support * 1.002) {
        signal = "📈 BUY ZONE (Gold near Support)";
    }
    else if (lastPrice >= resistance * 0.998) {
        signal = "📉 SELL ZONE (Gold near Resistance)";
    }
    else {
        signal = "⏳ WAIT (No clear zone)";
    }

    document.getElementById("goldSignal").innerText =
        "Support: " + support.toFixed(2) +
        " | Resistance: " + resistance.toFixed(2) +
        "\n" + signal;
  function drawLevels() {
    let dataInput = document.getElementById("priceData").value;
    let prices = dataInput.split(",").map(Number);

    let canvas = document.getElementById("chart");
    let ctx = canvas.getContext("2d");

    ctx.clearRect(0, 0, canvas.width, canvas.height);

    let max = Math.max(...prices);
    let min = Math.min(...prices);

    // Draw price line
    ctx.beginPath();
    prices.forEach((p, i) => {
        let x = i * 30;
        let y = canvas.height - ((p - min) / (max - min)) * canvas.height;

        if (i === 0) ctx.moveTo(x, y);
        else ctx.lineTo(x, y);
    });
    ctx.strokeStyle = "white";
    ctx.stroke();

    // Support = lowest
    let support = min;

    // Resistance = highest
    let resistance = max;

    // Draw Support Line
    let supportY = canvas.height - ((support - min) / (max - min)) * canvas.height;
    ctx.strokeStyle = "green";
    ctx.beginPath();
    ctx.moveTo(0, supportY);
    ctx.lineTo(canvas.width, supportY);
    ctx.stroke();

    // Draw Resistance Line
    let resY = canvas.height - ((resistance - min) / (max - min)) * canvas.height;
    ctx.strokeStyle = "red";
    ctx.beginPath();
    ctx.moveTo(0, resY);
    ctx.lineTo(canvas.width, resY);
    ctx.stroke();
}
  let questions = [
    {
        q: "What is Support?",
        options: ["Price stops falling", "Price goes up fast"],
        answer: 0
    },
    {
        q: "What is Resistance?",
        options: ["Price stops rising", "Price goes down fast"],
        answer: 0
    },
    {
        q: "What is Uptrend?",
        options: ["Higher High + Higher Low", "Lower High + Lower Low"],
        answer: 0
    },
    {
        q: "Where to place Stop Loss (Buy)?",
        options: ["Below support", "Above resistance"],
        answer: 0
    },
    {
        q: "Hammer candle means?",
        options: ["Bullish reversal", "Bearish trend"],
        answer: 0
    },
    {
        q: "Shooting star means?",
        options: ["Bearish reversal", "Bullish continuation"],
        answer: 0
    },
    {
        q: "Best Risk Reward?",
        options: ["1:2 or higher", "1:1"],
        answer: 0
    },{
    q: "Your question?",
    options: ["Option 1", "Option 2"],
    answer: 0
},
    {
        q: "EMA shows?",
        options: ["Trend", "Volume"],
        answer: 0
    },
    {
        q: "Green candle means?",
        options: ["Price up", "Price down"],
        answer: 0
    },
    {
        q: "Red candle means?",
        options: ["Price down", "Price up"],
        answer: 0
    }
];


// GENERATE QUIZ
let quizBox = document.getElementById("quizBox");


questions.forEach((item, index) => {
    let html = `<p>${index + 1}. ${item.q}</p>`;
    
    item.options.forEach((opt, i) => {
        html += `
        <label>
            <input type="radio" name="q${index}" value="${i}">
            ${opt}
        </label><br>`;
    });

    quizBox.innerHTML += html;
});

// CHECK SCORE
function submitQuiz() {
    let score = 0;

    questions.forEach((item, index) => {
        let selected = document.querySelector(`input[name="q${index}"]:checked`);
        
        if (selected && parseInt(selected.value) === item.answer) {
            score++;
        }
    });

    document.getElementById("scoreResult").innerText =
        "Your Score: " + score + " / " + questions.length;
}
function toggle(id) {
    let el = document.getElementById(id);
    el.style.display = el.style.display === "block" ? "none" : "block";
    function calculateProfit() {
    let buy = parseFloat(document.getElementById("buyPrice").value);
    let sell = parseFloat(document.getElementById("sellPrice").value);
    let qty = parseFloat(document.getElementById("quantity").value);
    let sl = parseFloat(document.getElementById("slPrice").value);
    let target = parseFloat(document.getElementById("targetPrice").value);

    let profit = (sell - buy) * qty;

    // Risk Reward Calculation
    let risk = Math.abs(buy - sl);
    let reward = Math.abs(target - buy);

    let rr = (reward / risk).toFixed(2);

    let resultText = "";

    if (profit > 0) {
        resultText = "Profit: ₹" + profit;
    } else if (profit < 0) {
        resultText = "Loss: ₹" + profit;
    } else {
        resultText = "No Profit No Loss";
    }

    resultText += " | R:R = 1 : " + rr;

    document.getElementById("profitResult").innerText = resultText;
    
}
}
function calculateProfit() {
    let buy = document.getElementById("buyPrice").value;
    let sell = document.getElementById("sellPrice").value;
    let qty = document.getElementById("quantity").value;

    let profit = (sell - buy) * qty;

    let resultText = "";

    if (profit > 0) {
        resultText = "Profit: ₹" + profit;
    } else if (profit < 0) {
        resultText = "Loss: ₹" + profit;
    } else {
        resultText = "No Profit No Loss";
    }

    document.getElementById("profitResult").innerText = resultText;
}
function check(btn, ans) {
    if(ans === "correct") {
        btn.style.background = "green";
        document.getElementById("result").innerText = "✅ Correct";
    } else {
        btn.style.background = "red";
        document.getElementById("result").innerText = "❌ Wrong";
    }
}
</script>

let timeLeft = 60; // seconds
let timerDisplay = document.getElementById("timer");

let timer = setInterval(() => {
    timeLeft--;
    timerDisplay.innerText = "Time Left: " + timeLeft + "s";

    if (timeLeft <= 0) {
        clearInterval(timer);
        submitQuiz(); // auto submit
        alert("⏱️ Time's up! Quiz submitted.");
    }
}, 1000);

</body>
</html>
<div class="card">
    <h3>📒 Trading Journal</h3>

    <input type="text" id="pair" placeholder="Pair (BTC/USDT)" style="width:100%; padding:8px;"><br><br>
    <input type="number" id="entry" placeholder="Entry Price" style="width:100%; padding:8px;"><br><br>
    <input type="number" id="sl" placeholder="Stop Loss" style="width:100%; padding:8px;"><br><b
    r>
      <div class="card">
    <h3>💰 Profit / Loss Calculator</h3>

    <input type="number" id="buyPrice" placeholder="Buy Price"><br><br>
    <input type="number" id="sellPrice" placeholder="Sell Price"><br><br>
    <input type="number" id="quantity" placeholder="Quantity"><br><br>

    <button onclick="calculateProfit()">Calculate</buttonfunction calculateProfit() {
    let buy = parseFloat(document.getElementById("buyPrice").value);
    let sell = parseFloat(document.getElementById("sellPrice").value);
    let qty = parseFloat(document.getElementById("quantity").value);
    let sl = parseFloat(document.getElementById("slPrice").value);
    let target = parseFloat(document.getElementById("targetPrice").value);

    let profit = (sell - buy) * qty;

    let risk = Math.abs(buy
