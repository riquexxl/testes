# testes
estudo

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto 001</title>
    <style>
        body {
            background-image: url(image/gifzada.gif);
            background-size: cover;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
            
        a {
            text-decoration: none;
        }
        .box {
            font-size: 20px;
            color: white;
            height: 250px;
            width: 350px;
            background: #191919;
            flex-direction: column;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .buttons-container {
            display: flex;
            justify-content: space-around;
            height: 50px;
            width: 150px;
        }
        button {
            height: 30px;
            width: 50px;
            background: white;
            border-radius: 5px;
            color: rgb(0, 0, 0);
            font-size: 16px; 
        }
    </style>
</head>
<body>
    <div class="box">
        <p>Se increva no canal</p>
        <div class="buttons-container">
            <button>
                <a href="https://www.youtube.com/@hnq.riquexL/featured">Sim</a>
            </button>
            <button id="nao">Não</button> 
        </div>
    </div>
</body>
<script>
    let button = document.getElementById('nao'); 
    let height = window.innerHeight - 50;
    let width = window.innerWidth - 50;

    button.addEventListener('mouseover', function() {
        button.style.position = "absolute"; 
        button.style.top = Math.random() * height + "px"; 
        button.style.left = Math.random() * width + "px";
    });
</script>
</html>
