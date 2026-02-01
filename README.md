# OPEN-IT-HELEN
VALENTINES
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💘</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
      background-color: #ffe6f0;
    }
    h1 {
      font-size: 2.5em;
    }
    button {
      font-size: 20px;
      padding: 12px 25px;
      margin: 20px;
      cursor: pointer;
      position: relative;
    }
    #noBtn {
      position: absolute;
    }
  </style>
</head>
<body>

<h1>Will you be my Valentine? 💖</h1>

<button onclick="yesClicked()">Yes 💕</button>
<button id="noBtn">No 💔</button>

<script>
  const noBtn = document.getElementById("noBtn");

  noBtn.addEventListener("mouseover", () => {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 100);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });

  function yesClicked() {
    document.body.innerHTML = "<h1>Yay!! 💘🥰</h1><p>Best choice ever.</p>";
  }
</script>

</body>
</html>
