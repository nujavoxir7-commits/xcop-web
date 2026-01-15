<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>XCOP Coin</title>
<style>
body {
  background: #0f1220;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-family: Arial;
}
#coin {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  background: gold;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 32px;
  cursor: pointer;
  user-select: none;
}
#count {
  position: absolute;
  top: 20px;
  font-size: 24px;
}
</style>
</head>
<body>

<div id="count">XCOP: 0</div>
<div id="coin">🪙</div>

<script>
let count = 0;
document.getElementById("coin").onclick = () => {
  count++;
  document.getElementById("count").innerText = "XCOP: " + count;
};
</script>

</body>
</html>
