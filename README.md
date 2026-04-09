# Caccia-al-tesoro-
<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <title>Caccia al tesoro</title>
  <style>
    body { font-family: Arial; text-align: center; margin-top: 100px; }
    #contenuto { display: none; }
  </style>
</head>
<body>

<h2>Inserisci la password</h2>
<input type="password" id="password">
<button onclick="controlla()">Entra</button>

<p id="errore" style="color:red;"></p>

<div id="contenuto">
  <h1>Hai trovato l’indizio! 🎉</h1>
  <p>Prossima tappa: guarda sotto il tavolo...</p>
</div>

<script>
function controlla() {
  let pass = document.getElementById("password").value;

  if(pass === "roma") {
    document.getElementById("contenuto").style.display = "block";
    document.getElementById("errore").innerText = "";
  } else {
    document.getElementById("errore").innerText = "Password sbagliata!";
  }
}
</script>

</body>
</html>
