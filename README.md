<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Caring Messages</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Pacifico&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: #f7f2f9;
      color: #3e3e3e;
    }
    
    /* Frame and Navigation Bar */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
      background-color: #ffffff;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      border-radius: 10px;
    }
    
    .navbar {
      background-color: #f8b0d0;
      padding: 15px;
      border-radius: 10px;
      display: flex;
      justify-content: space-around;
      margin-bottom: 20px;
    }

    .navbar a {
      text-decoration: none;
      color: #ffffff;
      font-size: 18px;
      font-weight: bold;
      padding: 8px 15px;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    .navbar a:hover {
      background-color: #f7a3c5;
    }

    /* Button for message */
    .message-button {
      background-color: #D8A7F5;
      color: white;
      padding: 15px 25px;
      font-size: 1.2em;
      border-radius: 30px;
      cursor: pointer;
      border: none;
      transition: transform 0.3s ease;
    }

    .message-button:hover {
      transform: scale(1.1);
    }

    /* Message display area */
    .message-box {
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      margin-top: 20px;
      display: none;
    }

    .message-box p {
      font-size: 1.2em;
      color: #5e4b8b;
      font-family: 'Pacifico', cursive;
    }

    /* About and Contact Sections */
    .section {
      margin-top: 30px;
      padding: 20px;
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .section h2 {
      font-family: 'Pacifico', cursive;
      color: #D8A7F5;
    }

    /* Cute Icon */
    .icon {
      font-size: 2em;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Navigation Bar -->
    <div class="navbar">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </div>

    <!-- Home Section -->
    <div id="home">
      <h1>Welcome to the Kawaii Corner</h1>
      <p>Click the cute buttons for caring messages!</p>

      <!-- Buttons for different messages -->
      <button class="message-button" onclick="showMessage('message1')">Message 1 💖</button>
      <button class="message-button" onclick="showMessage('message2')">Message 2 🌟</button>
      <button class="message-button" onclick="showMessage('message3')">Message 3 ✨</button>

      <!-- Message Box (Initially Hidden) -->
      <div class="message-box" id="message-box">
        <p id="message">You're doing great! Keep going, and don't forget to smile 😊</p>
      </div>

      <!-- Cute Icon -->
      <div class="icon" onclick="showMessage('message1')">🌸</div>
    </div>

    <!-- About Section -->
    <div id="about" class="section">
      <h2>About Us</h2>
      <p>This website was created with the intention of spreading kindness and positive energy. Our goal is to give you a moment of happiness and help brighten your day!</p>
      <p>Here, you can get cute messages, interact with fun content, and just take a moment to enjoy some kawaii vibes.</p>
    </div>

    <!-- Contact Section -->
    <div id="contact" class="section">
      <h2>Contact Us</h2>
      <p>If you have any questions or just want to say hi, feel free to reach out!</p>
      <p>Email us at: <a href="mailto:info@example.com">info@example.com</a></p>
    </div>
  </div>

  <script>
    function showMessage(messageId) {
      const messageBox = document.getElementById("message-box");
      const message = document.getElementById("message");

      // Switch between messages based on the button clicked
      if (messageId === 'message1') {
        message.innerHTML = "You're doing amazing! Keep it up! 💖";
      } else if (messageId === 'message2') {
        message.innerHTML = "You are full of potential! ✨";
      } else if (messageId === 'message3') {
        message.innerHTML = "Believe in yourself, you are capable of great things! 🌟";
      }

      // Show the message box
      messageBox.style.display = "block";
    }
  </script>
</body>
</html>
