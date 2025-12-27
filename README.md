<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Android 5.0 Lollipop</title>

<style>
body{
  margin:0;
  background:#bdbdbd;
  font-family: Roboto, Arial, sans-serif;
}

/* Telefone */
#phone{
  width:360px;
  height:640px;
  margin:20px auto;
  background:#f5f5f5;
  border-radius:18px;
  box-shadow:0 0 15px #0006;
  overflow:hidden;
}

/* Barra superior */
#status{
  height:24px;
  background:#0288d1;
  color:white;
  font-size:12px;
  padding:4px 8px;
}

/* Home */
#home{
  padding:15px;
}

.icon{
  width:72px;
  height:72px;
  background:white;
  border-radius:14px;
  display:inline-flex;
  align-items:center;
  justify-content:center;
  margin:10px;
  font-size:28px;
  cursor:pointer;
}

/* Apps */
.app{
  display:none;
  padding:10px;
}

button{
  padding:6px 10px;
}
</style>
</head>

<body>

<div id="phone">

  <div id="status">Android 5.0</div>

  <!-- HOME -->
  <div id="home">
    <div class="icon" onclick="openApp('browser')">🌐</div>
    <div class="icon" onclick="openApp('contacts')">👥</div>
  </div>

  <!-- NAVEGADOR -->
  <div id="browser" class="app">
    <button onclick="goHome()">⬅</button>
    <h3>Navegador</h3>
    <input id="url" placeholder="wikipedia.org" style="width:95%">
    <button onclick="go()">Ir</button>
    <iframe id="web"
      style="width:100%; height:480px; border:none;">
    </iframe>
  </div>

  <!-- CONTATOS -->
  <div id="contacts" class="app">
    <button onclick="goHome()">⬅</button>
    <h3>Contatos</h3>
    <p>Ana Lima – (11) 91234-5678</p>
    <p>Bruno Souza – (21) 99876-543
