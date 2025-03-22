<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barışalım mı?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            margin-top: 50px;
        }
        #container {
            position: relative;
            display: inline-block;
        }
        button {
            font-size: 20px;
            padding: 10px;
            margin: 10px;
            cursor: pointer;
        }
        #hayir {
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Benimle barışır mısın?</h1>
    <div id="container">
        <button onclick="alert('Harika! ❤️')">Evet</button>
        <button id="hayir">Hayır</button>
    </div>

    <script>
        document.getElementById("hayir").addEventListener("mouseover", function() {
            let x = Math.random() * window.innerWidth * 0.8; 
            let y = Math.random() * window.innerHeight * 0.8;
            this.style.left = x + "px";
            this.style.top = y + "px";
        });
    </script>

</body>
</html>
