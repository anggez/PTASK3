
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        background-image: url(https://i.pinimg.com/736x/05/6a/30/056a308745af6de1b5f8b2161bda2774.jpg);
        background-repeat: no-repeat;
        text-align: center;
        text-shadow: 2px 2px rgb(192, 131, 17);
        background-position: center;
        background-size: 1000px;
        font-size: xx-large;
    }
    h1 {
        border-style: groove;
        border-width: 15px;
        border-color: bisque;
    }
    #id {
        border: ;
    }
</style>
</head>
<body>

    <h2>FUNCTIONS</h2>

    <button onclick="calculate()">Calculate</button>
    
    <p id="result"></p>
    
    <script>
    function calculate() {
        var numbers = [];
        var oddCount = 0;
        var evenCount = 0;
        var sum = 0;
    
        for (var i = 0; i < 25; i++) {
            var num = parseInt(prompt("Enter integer #" + (i + 1) + ":"));
            numbers.push(num);
            if (num % 2 === 0) {
                evenCount++;
            } else {
                oddCount++;
            }
            sum += num;
        }
    
        var resultMessage = "Odd numbers: " + oddCount + "<br>";
        resultMessage += "Even numbers: " + evenCount + "<br>";
        resultMessage += "Sum of all numbers: " + sum;
    
        document.getElementById("result").innerHTML = resultMessage;
    }
    </script>
    
</body>
</html>
