<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8" />  
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>  
<title>Will You Be My Valentine?</title>  
<style>  
  body {  
    margin: 0;  
    font-family: Arial, sans-serif;  
    background: linear-gradient(135deg, #ffd6e8, #ffeef5);  
    display: flex;  
    justify-content: center;  
    align-items: center;  
    height: 100vh;  
    text-align: center;  
  }  
  
  .card {  
    background: white;  
    padding: 40px;  
    border-radius: 20px;  
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);  
    max-width: 350px;  
  }  
  
  h1 {  
    font-size: 22px;  
    margin-bottom: 30px;  
  }  
  
  .buttons {  
    display: flex;  
    justify-content: center;  
    gap: 20px;  
  }  
  
  button {  
    border: none;  
    padding: 12px 25px;  
    border-radius: 25px;  
    font-size: 16px;  
    cursor: pointer;  
    transition: 0.2s ease;  
  }  
  
  #yesBtn {  
    background-color: #ff4d88;  
    color: white;  
  }  
  
  #noBtn {  
    background-color: #eee;  
  }  
  
  #message {  
    margin-top: 20px;  
    font-size: 18px;  
    color: #ff4d88;  
    font-weight: bold;  
  }  
</style>  
</head>  
<body>  
  
<div class="card">  
  <h1>✨ <span id="name">Nume</span>, will you be my Valentine? 💖</h1>  
    
  <div class="buttons">  
    <button id="yesBtn">Yes</button>  
    <button id="noBtn">No</button>  
  </div>  
  
  <div id="message"></div>  
</div>  
  
<script>  
  // 🔁 SCHIMBĂ NUMELE AICI  
  document.getElementById("name").textContent = "Dani";   
  
  const noBtn = document.getElementById("noBtn");  
  const yesBtn = document.getElementById("yesBtn");  
  const message = document.getElementById("message");  
  
  noBtn.addEventListener("mouseover", () => {  
    const x = Math.random() * 200 - 100;  
    const y = Math.random() * 200 - 100;  
    noBtn.style.transform = `translate(${x}px, ${y}px)`;  
  });  
  
  yesBtn.addEventListener("click", () => {  
    message.textContent = "YAYYY 💘 I knew it!!!";  
  });  
</script>  
  
</body>  
</html>  
