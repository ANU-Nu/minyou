<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>QR Code คิดถึง</title>
  <script src="https://cdn.jsdelivr.net/npm/qrcode/build/qrcode.min.js"></script>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      text-align: center;
      margin-top: 50px;
    }
    canvas {
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>ส่งความคิดถึง ❤️</h1>
  <p>สแกน QR Code ด้านล่าง</p>
  <div id="qrcode"></div>

  <script>
    const message = "คิดถึงนะ 😊";
    QRCode.toCanvas(document.getElementById("qrcode"), message, function (error) {
      if (error) console.error(error);
      else console.log("QR Code สร้างสำเร็จ!");
    });
  </script>
</body>
</html>
