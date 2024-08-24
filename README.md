<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Proposal for Sinchana</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f7e7e7;
            margin: 0;
            padding: 20px;
            text-align: center;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }

        h1 {
            color: #ff6b6b;
            font-size: 36px;
            margin-bottom: 20px;
        }

        #message {
            color: #555;
            font-size: 24px;
            margin-bottom: 20px;
            display: none;
        }

        #button-container {
            margin-top: 30px;
        }

        button {
            padding: 15px 25px;
            font-size: 18px;
            color: #fff;
            background-color: #ff6b6b;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #ff4b4b;
        }

        #finalMessage {
            font-size: 28px;
            color: #ff6b6b;
            display: none;
            margin-top: 20px;
        }

        #heart {
            font-size: 50px;
            color: #ff6b6b;
            display: none;
            animation: heartbeat 1.5s infinite;
            margin-top: 20px;
        }

        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }
    </style>
</head>
<body>
    <h1>Hey Sinchana, I've got something to ask...</h1>

    <div id="message">
        You make my days brighter and my heart warmer. <br> 
        I was wondering...
    </div>

    <div id="button-container">
        <button onclick="revealMessage()">Click here to find out</button>
    </div>

    <div id="finalMessage">Will you go out with me? 💖</div>
    <div id="heart">❤️</div>

    <script>
        function revealMessage() {
            document.getElementById('message').style.display = 'block';
            document.getElementById('button-container').style.display = 'none';

            setTimeout(function() {
                document.getElementById('finalMessage').style.display = 'block';
                document.getElementById('heart').style.display = 'block';
            }, 2000);
        }
    </script>
</body>
</html>
