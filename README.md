# Kavya-love
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Bangaru 💛</title>

<style>
body {
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
    color: white;
    text-align: center;
    overflow-x: hidden;
}

.container {
    padding: 20px;
    margin-top: 40px;
}

h1 {
    font-size: 28px;
    animation: fadeIn 2s ease-in-out;
}

h2 {
    font-size: 22px;
    margin-top: 20px;
}

p {
    font-size: 18px;
    margin: 20px 0;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 40px;
    background: white;
    color: #ff4081;
    cursor: pointer;
    transition: 0.3s;
}

button:hover {
    background: #ff4081;
    color: white;
}

.heart {
    font-size: 50px;
    animation: heartbeat 1.5s infinite;
}

.countdown {
    font-size: 20px;
    margin-top: 20px;
    font-weight: bold;
}

.hidden {
    display: none;
    margin-top: 20px;
    font-size: 20px;
}

@keyframes heartbeat {
    0% { transform: scale(1); }
    25% { transform: scale(1.2); }
    50% { transform: scale(1); }
    75% { transform: scale(1.2); }
    100% { transform: scale(1); }
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}
</style>
</head>

<body>

<div class="container">
    <div class="heart">💛</div>

    <h1>To My Bangaru, Kavya 💛</h1>

    <p>
        From the moment you came into my life,<br>
        everything became brighter and more meaningful.<br><br>
        Your smile is my peace,<br>
        your voice is my comfort,<br>
        and your love is my biggest strength.
    </p>

    <h2>⏳ Time Since I Fell For You</h2>
    <div class="countdown" id="countdown"></div>

    <br>
    <button onclick="showProposal()">Click Here Bangaru 💌</button>

    <div class="hidden" id="proposal">
        Kavya 💛<br><br>
        You are the only one I trust,<br>
        the only one my heart chooses every single day.<br><br>
        I promise to respect you, support you,<br>
        and stand beside you always.<br><br>
        💍 Will You Stay With Me Forever? 💛
    </div>
</div>

<!-- Romantic Instrumental Music -->
<audio autoplay loop>
  <source src="https://www2.cs.uic.edu/~i101/SoundFiles/CanonInD.mp3" type="audio/mpeg">
</audio>

<script>
// Set your love start date here (Change if needed)
var loveDate = new Date("2024-01-01").getTime();

var x = setInterval(function() {
  var now = new Date().getTime();
  var distance = now - loveDate;

  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  document.getElementById("countdown").innerHTML =
    days + " Days " + hours + " Hours "
    + minutes + " Minutes " + seconds + " Seconds 💛";

}, 1000);

function showProposal() {
    document.getElementById("proposal").style.display = "block";
}
</script>

</body>
</html>
