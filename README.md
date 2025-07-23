html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>العرش الحديدي</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', sans-serif;
      background: url('https://images.unsplash.com/photo-1579546929662-711aa81148cf?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80') no-repeat center center fixed;
      background-size: cover;
      color: white;
      text-align: center;
      min-height: 100vh;
    }
    .overlay {
      background: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 15px;
      max-width: 600px;
      margin: 20px auto;
    }
    h1 {
      font-size: 2.5em;
      color: #FFD700;
      text-shadow: 0 0 15px #FF4500;
      margin: 10px 0;
    }
    .designer {
      color: #aaa;
      font-size: 14px;
      margin-bottom: 20px;
    }
    .logo {
      width: 100px;
      margin: 0 auto 15px;
      animation: glow 2s infinite alternate;
    }
    @keyframes glow {
      0% { filter: drop-shadow(0 0 5px #FFD700); }
      100% { filter: drop-shadow(0 0 20px #FF4500); }
    }
    .resources {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin: 20px auto;
      background: rgba(0, 0, 0, 0.6);
      padding: 15px;
      border-radius: 15px;
    }
    .resource {
      text-align: center;
    }
    .resource span {
      font-size: 24px;
    }
    .upgrade-box {
      background: rgba(45, 26, 74, 0.9);
      border-radius: 15px;
      padding: 20px;
      max-width: 500px;
      margin: 30px auto;
      border: 1px solid #C19A6B;
    }
    .btn {
      background: #FF4500;
      color: white;
      border: none;
      padding: 15px 40px;
      font-size: 1.2em;
      border-radius: 50px;
      margin: 15px;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }
    .sorceress {
      position: fixed;
      bottom: 20px;
      left: 20px;
      width: 110px;
      animation: float 3s ease-in-out infinite;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0, 255, 200, 0.5);
    }
    .warrior {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 110px;
      animation: float 3s ease-in-out infinite;
      animation-delay: 0.5s;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(255, 69, 0, 0.5);
    }
    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }
  </style>
</head>
<body>

  <div class="overlay">
    <img src="https://i.ibb.co/6Xv0dVn/throne-logo.png" alt="شعار العرش الحديدي" class="logo">
    <h1>🔥 العرش الحديدي</h1>
    <p class="designer">تصميم: خالد يحيى مروعي الشاجري</p>

    <div class="resources">
      <div class="resource">
        <span>🩸</span>
        <b>دم الذهب</b>
        <div>1,250,000</div>
      </div>
      <div class="resource">
        <span>🔥</span>
        <b>روح النار</b>
        <div>980,000</div>
      </div>
      <div class="resource">
        <span>👑</span>
        <b>حديد العرش</b>
        <div>450,000</div>
      </div>
    </div>

    <div class="upgrade-box">
      <div>🚀 رامية العرش → المستوى 6</div>
      <div style="height:20px;background:#333;border-radius:10px;overflow:hidden;margin:10px 0">
        <div id="progress" style="width:0%;height:100%;background:#FF4500"></div>
      </div>
      <div id="time">الوقت: 06:00:00</div>
    </div>

    <button class="btn" onclick="attack()">⚔️ هاجم الآن</button>
  </div>

  <!-- لمياء الشاجريّة -->
  <img src="https://i.ibb.co/0jz0Z9L/shajariya.png" alt="لمياء الشاجريّة" class="sorceress">
  
  <!-- عبد العزيز -->
  <img src="https://i.ibb.co/SdGqWcX/abdulaziz.png" alt="عبد العزيز" class="warrior"># -
