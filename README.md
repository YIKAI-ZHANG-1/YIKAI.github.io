# This is my GitHub page 
By YIKAI ZHANG
<!DOCTYPE html>
<html>
<head>
    <title>VAT Calculator</title>
    <script>
        function calculateVAT() {
            var grossPrice = parseFloat(document.getElementById("grossPrice").value);
            var vatRate = 0.07; // 7% VAT rate
            var vatAmount = grossPrice * vatRate;
            document.getElementById("vatAmount").textContent = vatAmount.toFixed(2);
        }
    </script>
</head>
<body>
    <h1>VAT Calculator</h1>
    <label for="grossPrice">Gross Price:</label>
    <input type="number" id="grossPrice" step="0.01">
    <button onclick="calculateVAT()">Calculate</button>
    <br>
    <label for="vatAmount">VAT Amount:</label>
    <span id="vatAmount"></span>
</body>
</html>
