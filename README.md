# stockify
Application de gestion de stock
<!DOCTYPE html> 
<html lang="fr">
<head>
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    
  <title>Stemar Accueil</title> 
    <style>
        body {
            background-color: lightgray;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
       img {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
        header {
            text-align: center;
            margin: 50px 0;
            font-size: 2em;
        }
        
        .container {
            display: flex;
            justify-content: center;
            background-color: black;
            padding: 10px 0;
        }
        
        .container button {
            background-color: black;
            color: white;
            border: none;
            padding: 10px 20px;
            margin: 0 10px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .container button:hover {
            background-color: #333333;
        }
    </style>
</head>
<body>
    
    <header>Stemar Accueil</header>
    
    <div class="container">
        <button onclick="location.href='Stemar_Materiel.html'">Stemar Materiel</button>
        <button onclick="location.href='Stemar_Client.html'">Stemar Client</button>
        <button onclick="location.href='Stemar_materiel2.html'">Stemar Client</button>
        
    </div>
   <br>
    <br>
    <img src="Stemar_logo.png" alt="Stemar_logo">
    <br>
    <!-- Encadré à droite -->
	<div class="encadre-droite">
		Alertes clients / Materiels
	</div>
	
	<div id="client-nom"></div>
	<script>
		const urlParams = new URLSearchParams(window.location.search);
		const clientNom = urlParams.get('client');
		const clientNomElement = document.getElementById('client-nom');
		clientNomElement.textContent = clientNom;
	</script>	
    <br>
</body>
</html>
