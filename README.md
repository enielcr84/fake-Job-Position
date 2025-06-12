<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Job Offer Application Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      padding: 20px;
    }
    .container {
      background-color: #fff;
      max-width: 500px;
      margin: auto;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    h2 {
      text-align: center;
    }
    input[type="text"], input[type="email"] {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    input[type="submit"] {
      background-color: #007BFF;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .message {
      margin-top: 20px;
      padding: 15px;
      background-color: #ffdddd;
      border-left: 6px solid #f44336;
    }
    .logo {
      width: 150px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4e/Microsoft_logo.svg/512px-Microsoft_logo.svg.png" alt="Company Logo" class="logo">
    <h2>Apply for Our Job Offer</h2>
    <form onsubmit="showMessage(); return false;">
      <label>Name:</label>
      <input type="text" name="name" required>

      <label>Email:</label>
      <input type="email" name="email" required>

      <label>Phone:</label>
      <input type="text" name="phone" required>

      <input type="submit" value="Submit">
    </form>

    <div id="message" class="message" style="display:none;">
      <strong>Warning!</strong> This was a QR code phishing simulation. Never scan codes from unverified sources. This form did not collect any information.
    </div>
  </div>

  <script>
    function showMessage() {
      document.getElementById('message').style.display = 'block';
    }
  </script>
</body>
</html>
