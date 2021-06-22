# Curr-currículo pagina web. e chat box.
<!doctype html>
<!DOCTYPE html>
<html>
<head>
	<title>Curriculo</title>
	<link rel="stylesheet" type="text/css" href="css/style.css"/>

  <meta name="viewport" content="width=device-widht, initial-scale=1.0, maximun-scale=1.0">
	<meta charset="utf-8/">
  <style type="text/css">
  </style>
</head>
<body>
  <div class="header">
      <h1>Kleberton Ferreirea Santos de Jesus Ribeiro</h1>
	 <div class="center">
    <img src="imagens/foto.jpg" width="100" height="140">
     </div><!--center-->
  </div><!--header-->
  <div class="container-banner">
  	 <div class="center">
       <div class="menu">
          <div class="container">
            <div class="topnav">
              <a href="#formacao">Formação</a>
              <a href="#projetos">Projetos</a>
              <a href="#contato">Contato</a>
            </div>
          </div>
       </div>
         <div>
            <button class="open-button" onclick="openForm()">ChatBox</button>
         </div>
       <div class="chat-popup" id="myForm">
          <form action="/action_page.php" class="form-container">
             <h1>ChatBox</h1>
             <label for="msg"><b>Mensagem...</b></label>
             <textarea placeholder="Digite a mensagem.." name="msg" required></textarea>
             <button type="submit" class="btn">Enviar</button>
             <button type="button" class="btn cancel" onclick="closeForm()">Fechar</button>
          </form>
      </div>
 <script>
    function openForm() {
    document.getElementById("myForm").style.display = "block";
   }

   function closeForm() {
   document.getElementById("myForm").style.display = "none";
   }
</script>
  	 	</div><!--form-->
  	</div><!--center--> 		
  </div><!--container-banner-->
</body>
</html>
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
img{
	clip-path: circle(50%);
	margin-left: 10px;
}
html,body{
	height: 100%;
}
.header>h1{
	width: 1280px;
	margin:center;
	color: white;
	height:100%
}
.container{
	position: absolute;
	margin: 20px;
	width: auto;
	padding-left: 235px;
}
.topnav{
	overflow: hidden;
	background-color: #333;
}
.topnav a {
	float: left;
	color: #f2f2f2;
	text-align: center;
	padding: 14px 16px;
	text-decoration: none;
	font-size: 17px;
}
.topnav a.hover{
	background-color: #ddd;
	color: black;
}

.header {
	width: 100%;
	height: 60px;
	background-image:url('../imagens/backgroud.png.png');

}

.container-banner{
	width: 100%;
	height: 550px;
	margin: auto;
	background-image: url('../imagens/backgroud.png.png');
	background-size: cover;
	background-position: center;

}
.open-button {
  background-color: #333;
  color: white;
  padding: 16px 20px;
  border: none;
  cursor: pointer;
  opacity: 0.8;
  position: fixed;
  bottom: 23px;
  right: 28px;
  width: 280px;
}
.chat-popup {
  display: none;
  position: fixed;
  bottom: 0;
  right: 15px;
  border: 3px solid #f1f1f1;
  z-index: 9;
}
.form-container {
  max-width: 300px;
  padding: 10px;
  background-color: #A4A4A4;
}
.form-container textarea {
  width: 100%;
  padding: 15px;
  margin: 5px 0 22px 0;
  border: none;
  background: #f1f1f1;
  resize: none;
  min-height: 200px;
}
.form-container textarea.focus {
  background-color: #ddd;
  outline: none;
}
.form-container .btn {
  background-color: #04AA6D;
  color: white;
  padding: 16px 20px;
  border: none;
  cursor: pointer;
  width: 100%;
  margin-bottom:10px;
  opacity: 0.8;
}
.form-container .cancel {
  background-color: red;
}
.form-container .btn.hover, .open-button.hover {
  opacity: 1;
}
