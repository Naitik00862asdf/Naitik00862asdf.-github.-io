<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            background-color: #ffb6c1;
            font-family: 'Arial', sans-serif;
            text-align: center;
            padding: 50px;
        }
        h1 {
            font-size: 40px;
            color: #d10068;
            animation: glow 1.5s infinite alternate;
        }
        @keyframes glow {
            from { text-shadow: 0 0 10px #ff1493; }
            to { text-shadow: 0 0 20px #ff69b4; }
        }
        p {
            font-size: 20px;
            color: #650034;
        }
        .container {
            margin-top: 50px;
        }
        button {
            font-size: 20px;
            padding: 15px 30px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            margin: 20px;
            transition: 0.3s;
        }
        #yes {
            background-color: #ff1493;
            color: white;
        }
        #yes:hover {
            background-color: #ff69b4;
        }
        #no {
            background-color: #333;
            color: white;
            position: absolute;
        }
        #made-with-love {
            margin-top: 30px;
            font-size: 16px;
            color: #650034;
            font-style: italic;
        }
    </style>
</head>
<body>

    <h1>Hey Beautiful, Will You Be My Valentine? ❤️</h1>
    <p>I made this just for you! It took me so many hours! 😭</p>

    <div class="container">
        <button id="yes" onclick="showLoveMessage()">Yes ❤️</button>
        <button id="no" onmouseover="moveNoButton()">No 😢</button>
    </div>

    <p id="response" style="font-size: 25px; font-weight: bold; color: #ff1493;"></p>

    <p id="made-with-love">Made with ❤️ by Netik</p>

    <script>
        function showLoveMessage() {
            document.getElementById("response").innerHTML = "Yay! You said Yes! 🥰💖";
        }

        function moveNoButton() {
            let x = Math.random() * (window.innerWidth - 200);
            let y = Math.random() * (window.innerHeight - 100);
            document.getElementById("no").style.left = `${x}px`;
            document.getElementById("no").style.top = `${y}px`;
        }
    </script>

</body>
</html>
