# ZYGAL-Assignment--Nov-22
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    
        <link rel="stylesheet" href="task.css">
    
</head>
<body>
    <p id=red>1</p>
    <p id="yellow">2</p>
    <p id="green">3</p>
    <p id="orange">4</p>
    <button onclick="changeStyleClockwise()">Clockwise</button>
    <button onclick="changeStyleAntiClockwise()">Anticlockwise</button>
</body>
<script src="task.js"></script>
</html>

p{
    display: flex;

}
#red {
    background-color: red;
    display: inline-block;
    height:150px;
    width:150px;
    
}
#yellow {
    background-color: yellow;
    display: inline-block;
    height:150px;
    width:150px;
}
#green {
    background-color: green;
    display:inline-block;
    flex-direction: column;
    height:150px;
    width:150px;

}
#orange {
    background-color:orange;
    display: inline-block;
    height:150px;
    width:150px;
}

function changeStyleClockwise(){
    document.getElementById('red').style.backgroundColor='orange';
    document.getElementById('yellow').style.backgroundColor='red';
    document.getElementById('green').style.backgroundColor='yellow';
    document.getElementById('orange').style.backgroundColor='green';
}  

function changeStyleAntiClockwise(){

   document.getElementById('orange').style.backgroundColor='red';
   document.getElementById('green').style.backgroundColor='orange';
   document.getElementById('yellow').style.backgroundColor='green';
   document.getElementById('red').style.backgroundColor='yellow';
  
}
