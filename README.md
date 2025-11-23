# Heal-with-me
It's my hoppy to listen and heal everyone's hurts and to chill out with your <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Healing Space</title>
  <style>
    body {
      background: #e0f7fa;
      color: #004d40;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      padding: 20px;
      text-align: center;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 0.5em;
    }
    #quote {
      font-size: 1.5em;
      font-style: italic;
      max-width: 600px;
    }
    footer {
      position: absolute;
      bottom: 15px;
      font-size: 0.9em;
      color: #00796b;
    }
    button {
      margin-top: 2em;
      padding: 10px 20px;
      font-size: 1em;
      background-color: #004d40;
      color: #e0f7fa;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #00796b;
    }
  </style>
</head>
<body>
  <h1>Welcome to Your Healing Space</h1>
  <div id="quote">Loading your daily inspiration...</div>
  <button onclick="showQuote()">New Quote</button>
  
  <footer>May peace and healing find you.</footer>

  <script>
    const quotes = [
      "“Healing takes courage, and we all have courage, even if we have to dig a little to find it.” – Tori Amos",
      "“Sometimes the smallest step in the right direction ends up being the biggest step of your life.”",
      "“Your present circumstances don’t determine where you can go; they merely determine where you start.”",
      "“Self-care is how you take your power back.” – Lalah Delia",
      "“You are deserving of healing and happiness.”"
    ];

    function showQuote() {
      const index = Math.floor(Math.random() * quotes.length);
      document.getElementById('quote').textContent = quotes[index];
    }

    // Show a quote when page loads
    window.onload = showQuote;
  </script>
</body>
</html>
