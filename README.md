<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Anchal ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffcccb;
        }
        h1 {
            margin-top: 20%;
        }
        .buttons {
            margin-top: 20px;
        }
        .btn {
            padding: 10px 20px;
            font-size: 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: 0.3s;
        }
        #yes {
            background-color: #28a745;
            color: white;
        }
        #no {
            background-color: #dc3545;
            color: white;
            position: absolute;
        }
        .hidden {
            display: none;
        }
        .love-message {
            font-size: 24px;
            color: #ff0000;
        }
    </style>
</head>
<body>

    <h1>Do you love me, Anchal? ❤️</h1>
    <div class="buttons">
        <button id="yes" class="btn">Yes</button>
        <button id="no" class="btn">No</button>
    </div>

    <div id="message" class="hidden">
        <h2 class="love-message">Yay! Happy Valentine's Day, Anchal! 💖🌹</h2>
        <img src="https://media.giphy.com/media/3o7abKhOpu0NwenH3O/giphy.gif" alt="Love Gif">
    </div>

    <script>
        let noBtn = document.getElementById("no");
        let yesBtn = document.getElementById("yes");
        let messageDiv = document.getElementById("message");

        noBtn.addEventListener("mouseover", function () {
            let x = Math.floor(Math.random() * (window.innerWidth - 100));
            let y = Math.floor(Math.random() * (window.innerHeight - 100));
            noBtn.style.left = x + "px";
            noBtn.style.top = y + "px";
        });

        yesBtn.addEventListener("click", function () {
            document.querySelector(".buttons").style.display = "none";
            messageDiv.classList.remove("hidden");
        });
    </script>

</body>
</html>
