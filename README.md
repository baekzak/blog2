<!단진자>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>단진자 애니메이션</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }

        .pendulum-container {
            position: relative;
            width: 200px;
            height: 400px;
        }

        .pendulum {
            width: 4px;
            height: 200px;
            background: #333;
            position: absolute;
            top: 0;
            left: 50%;
            transform-origin: top;
            animation: swing 2s infinite ease-in-out;
        }

        .weight {
            width: 40px;
            height: 40px;
            background: #007acc;
            border-radius: 50%;
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }

        @keyframes swing {
            0% { transform: rotate(-30deg); }
            50% { transform: rotate(30deg); }
            100% { transform: rotate(-30deg); }
        }
    </style>
</head>
<body>
    <div class="pendulum-container">
        <div class="pendulum">
            <div class="weight"></div>
        </div>
    </div>
</body>
</html>
