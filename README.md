#<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="style.css">
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Interest Calculator</title>
</head>
<body>
    <div class="container">
        <h1>Simple Interest Calculator</h1>
        <div class="inpSection">
            <div class="amt">
                <label for="amount">Enter Total Amount:   </label>
                <input type="number" name="amount" id="amount" placeholder="Enter Total Amount">
            </div>
            <div class="time">
                <label for="time">Enter Time:   </label>
                <input type="number" name="time" id="time" placeholder="Enter Time">
            </div>
            <div class="rate">
                <label for="rate">Rate: </label>
                <input type="number" name="rate" id="rate" placeholder="Enter Rate">
            </div>
            <div class="button">
                <button onclick="Calculate()">Calculate</button>
            </div>
            <div class="result">
                <h3 id="si"></h3>
            </div>
        </div>
    </div>
    
</body>
<script>
    function Calculate()
    {
        let p=document.getElementById('amount').value;
        let t=document.getElementById('time').value;
        let r=document.getElementById('rate').value;
let  SI=(p*t*r)/100;

        document.getElementById('si').innerHTML="The Total Simple Intrest Is: "+SI;
    }
</script>
</html>
