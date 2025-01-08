<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pollution Monitoring Site</title>
  <link rel="stylesheet" href="style.css"> <!-- Link to your CSS file -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Poppins:wght@500;700&display=swap" rel="stylesheet">
</head>
<body>
  <header>
    <h1>🌍 Pollution Monitoring Site</h1>
  </header>
  <div class="container">
    <div class="search-bar">
      <input type="text" placeholder="Enter your location..." id="location-input">
      <button onclick="searchPollution()">🔍 Search</button>
    </div>
    <div class="pollution-data">
      <h2>Pollution Data</h2>
      <div class="card">
        <p><strong>📍 Location:</strong> <span id="location">N/A</span></p>
        <p><strong>🌫️ AQI:</strong> <span id="aqi">N/A</span></p>
        <p><strong>🌀 PM2.5:</strong> <span id="pm25">N/A</span></p>
        <p><strong>🌬️ PM10:</strong> <span id="pm10">N/A</span></p>
        <p><strong>🔊 Noise Level (dB):</strong> <span id="noise">N/A</span></p>
      </div>
    </div>
  </div>
  <footer>
    <p>🌟 Powered by Environmental Awareness | Designed with ❤️</p>
  </footer>
  <script>
    function searchPollution() {
      // Placeholder for functionality to fetch and display pollution data
      const location = document.getElementById("location-input").value;
      document.getElementById("location").textContent = location || "Unknown";
      document.getElementById("aqi").textContent = Math.floor(Math.random() * 500); // Simulated air data
      document.getElementById("pm25").textContent = (Math.random() * 100).toFixed(2);
      document.getElementById("pm10").textContent = (Math.random() * 150).toFixed(2);
      document.getElementById("noise").textContent = (Math.random() * 120).toFixed(2); // Simulated noise data
    }
  </script>
</body>
</html>
