# -mrk-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Surprise</title>
    <style>
        #messageBox {
            width: 200px;
            height: 200px;
            background-color: #fcc;
            overflow: hidden;
            transition: height 1s ease-in-out;
        }
    </style>
</head>
<body>
    <div id="messageBox">
        <h1 style="display: none;">Happy Valentine's Day!</h1>
        <p style="display: none;">You're special to me. Click the button to reveal the message.</p>
    </div>
    <button onclick="revealMessage()">Open Box</button>

    <script>
        function revealMessage() {
            const box = document.getElementById('messageBox');
            const title = box.querySelector('h1');
            const message = box.querySelector('p');

            title.style.display = 'block';
            message.style.display = 'block';

            // Simulate an "open box" effect
            box.style.height = 'auto';
        }
    </script>
</body>
</html>
