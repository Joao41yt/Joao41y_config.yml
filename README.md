<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: 'Montserrat', sans-serif;
            background-color: #191919;
            color: #f7df1e;
        }
        a {
            text-decoration: none;
            color: #f7df1e;
        }
        .box {
            font-size: 30px;
            border-radius: 10px;
            background: #191919;
            text-align: center;
            padding: 20px;
        }
        .buttons-container {
            display: flex;
            justify-content: space-around;
            margin-top: 20px;
        }
        button {
            height: 40px;
            width: 100px;
            background: white;
            color: black;
            font-weight: 600;
            border: 2px solid black;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="box">
        <p>BORA FICAR HOJE?</p>
        <div class="buttons-container">
            <button><a href="https://www.youtube.com/watch?v=MDmcVLadrmY">Sim</a></button>
            <button id="no">Não</button>
        </div>
    </div>

    <script>
        let button = document.getElementById('no');
        let height = window.innerHeight - 100;
        let width = window.innerWidth - 100;

        button.addEventListener('mouseover', function() {
            button.style.position = "absolute";
            button.style.top = Math.random() * height + "px";
            button.style.left = Math.random() * width + "px";
        });
    </script>
</body>
</html>
