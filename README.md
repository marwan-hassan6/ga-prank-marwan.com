<!DOCTYPE html>
<html>

<head>
    <title>Marwan's prank</title>
    <h1>
        <center><b>Are you gay ?</b></center>
    </h1>
    <style>
        #no-button {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
        
        #yes-button {
            position: absolute;
            top: 30%;
            left: 30%;
            transform: translate(-30%, -30%);
        }
    </style>
</head>

<body>
    <button id="yes-button" onclick="alert('Thank you!')">Yes</button>
    <button id="no-button" onmouseover="moveButton()">No</button>
    <script>
        function moveButton() {
            var button = document.getElementById("no-button");
            var x = Math.floor(Math.random() * window.innerWidth);
            var y = Math.floor(Math.random() * window.innerHeight);
            button.style.left = x + "px";
            button.style.top = y + "px";
        }
    </script>
</body>

</html>
