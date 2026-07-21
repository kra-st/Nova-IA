<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nova-IA</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f2f2f2;
}

header {
  background: #111827;
  color: white;
  text-align: center;
  padding: 20px;
  font-size: 28px;
}

#chat {
  height: 60vh;
  padding: 20px;
  overflow-y: auto;
}

.message {
  background: white;
  padding: 12px;
  margin: 10px;
  border-radius: 10px;
}

.box {
  display: flex;
  padding: 15px;
  background: white;
}

input {
  flex: 1;
  padding: 12px;
  font-size: 16px;
}

button {
  padding: 12px;
  background: #111827;
  color: white;
  border: none;
  margin-left: 5px;
}
</style>
</head>

<body>

<header>
🚀 Nova-IA
</header>

<div id="chat">
<div class="message">
Bienvenue sur Nova-IA 👋<br>
Pose-moi une question.
</div>
</div>

<div class="box">
<input id="question" placeholder="Écris ton message...">
<button onclick="envoyer()">Envoyer</button>
</div>

<script>
function envoyer(){
let q = document.getElementById("question").value;

if(q!=""){
document.getElementById("chat").innerHTML += 
"<div class='message'>👤 "+q+"</div>";

document.getElementById("chat").innerHTML += 
"<div class='message'>🤖 Nova-IA réfléchit... (version test)</div>";

document.getElementById("question").value="";
}
}
</script>

</body>
</html>
