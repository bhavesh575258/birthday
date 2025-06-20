<!doctype html>
<html lang="en">
    <head>
        <style>
            * {
                padding: 0;
                margin: 0;
            }
            body {
                background: pink;
                display: flex;
                justify-content: center;
                align-items: center;
                height: 100vh;
                font-family: 'Pacifico', cursive;
            }
            .main {
                text-align: center;
            }
            input {
                font-size: 30px;
                width: 200px;
                border: 2px solid red;
                border-radius: 20px;
                background: transparent;
                padding-left: 10px;
                margin-left: -20px; /* Shifts the input slightly to the left */
            }
            button {
                padding: 10px 20px;
                font-size: 30px;
                background: black;
                color: white;
                border: 2px solid gray;
                border-radius: 20px;
                cursor: pointer;
            }
            .content {
                display: none;
                text-align: center;
                font-size: 30px;
                text-shadow: 0 0 9px blue, 0 0 7px #fff, 0 0 10px #fff;
            }
            h1 {
                margin: 10px;
            }
        </style>
        <script>
            function show() {
                var name = document.getElementById('name').value;
                if (name == "") {
                    alert('Please type your name');
                } else {
                    document.getElementById('m1').style.display = "none";
                    document.getElementById('c1').style.display = "block";
                    document.getElementById('bhavesh').innerHTML = name;
                }
            }
        </script>
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Happy Birthday!</title>
    </head>
    <body>
        <div class="main" id="m1">
            <div>
                <h1>ENTER YOUR NAME</h1>
                <input type="text" placeholder="Enter Name" id="name">
                <br><br>
                <button onclick="show()">CLICK</button>
            </div>
        </div>
        <div class="content" id="c1">
            <h1>HAPPY</h1>
            <h1>BIRTHDAY</h1>
            <h1>DEAR</h1>
            <h1 id="bhavesh"></h1>
            <h1>🥳</h1>
        </div>
    </body>
</html>
