<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ZERO HUNGER</title>
    <style>
        /* Styles for the Zero Hunger page */
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://t3.ftcdn.net/jpg/02/92/07/56/360_F_292075696_hGdSBQ9Bvf1jsaVMP2rTpuRr0VMATck0.jpg');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            backdrop-filter: blur(5px);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 15px;
            width: 100%;
            position: fixed;
            top: 0;
            z-index: 1;
        }

        .navbar a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 4px;
            margin: 0 10px;
            transition: background-color 0.3s;
        }

        .navbar a:hover {
            background-color: #555;
        }

        .button-container {
            text-align: center;
            margin-top: 80px;
        }

        .custom-button {
            padding: 15px 30px;
            font-size: 18px;
            background-color: black;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin: 20px;
        }

        .custom-button:hover {
            background-color: green;
        }

        /* Styles for the Receiver Interface page */
        .receiver-container {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffffff7c;
            margin: 50;
            padding: 10;
        }

        .receiver-form {
            max-width: 400px;
            margin: 50px auto;
            padding: 20px;
            background-color: rgb(255, 255, 255);
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(9, 1, 54, 0.1);
        }

        .container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            display: flex;
            flex-direction: row;
            align-items: center;
        }

        label {
            display: block;
            margin-bottom: 8px;
        }

        input {
            width: 100%;
            padding: 8px;
            margin-bottom: 15px;
            box-sizing: border-box;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #d3b2d8;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #4d42a8;
        }

        .error {
            color: red;
            margin-top: 5px;
        }
    </style>
</head>

<body>
    <!-- Zero Hunger page content -->
    <div class="navbar">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
        <button class="close-button" onclick="closePage()">Close</button>
    </div>

    <div class="button-container">
        <button class="custom-button" onclick="redirectToDonorPage()">DONOR</button>
        <button class="custom-button" onclick="redirectToReceiverPage()">RECEIVER</button>
    </div>

    <!-- JavaScript logic for Zero Hunger page -->
    <script>
        function redirectToDonorPage() {
            window.location.href = 'wwwww.html';
        }

        function redirectToReceiverPage() {
            window.location.href = 'restrict.html';
        }

        function buttonClicked(buttonText) {
            alert(buttonText + " clicked!");
            // You can replace the alert with your desired action for each button
        }

        function closePage() {
            window.close();
        }
    </script>
    <script>
        function validateForm() {
            var phoneNumber = document.getElementById('phoneNumber').value;

            // Check if the phone number has 10 digits
            if (phoneNumber.length !== 10 || isNaN(phoneNumber)) {
                document.getElementById('phoneNumberError').innerHTML = 'Enter a valid 10-digit mobile number.';
                return false;
            } else {
                document.getElementById('phoneNumberError').innerHTML = '';
                return true;
            }
            
        }
    </script>
</body>
</html>
