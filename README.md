# Scarleth99   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dinosaurio y Tulipán</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #ffffff;
        }
        #dinosaur {
            position: relative;
            text-align: center;
        }
        #tulip {
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            transition: transform 2s;
        }
        #message {
            position: absolute;
            top: -50px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 24px;
            color: #000000;
        }
        img {
            max-width: 100%;
            height: auto;
        }
    </style>
</head>
<body>
    <div id="dinosaur">
        <img src="dinosaur.png" alt="Dinosaurio" id="dinoImg">
        <img src="tulip.png" alt="Tulipán" id="tulip">
        <div id="message">Eres preciosa my love</div>
    </div>

    <script>
        window.onload = function() {
            const tulip = document.getElementById('tulip');
            tulip.style.transform = 'translate(-50%, -100px)';
        };
    </script>
</body>
</html>
