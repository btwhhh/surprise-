<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Marry Me?</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: url('https://upload.wikimedia.org/wikipedia/commons/3/35/Engagement_ring_diamond.jpg') no-repeat center center fixed;
            background-size: cover;
            font-family: 'Arial', sans-serif;
        }

        .container {
            text-align: center;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }

        h1 {
            font-size: 3.5rem;
            animation: fadeIn 3s ease-in-out;
        }

        p {
            font-size: 1.5rem;
            margin-top: 10px;
            animation: fadeIn 5s ease-in-out;
        }

        .btn {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 30px;
            font-size: 1.5rem;
            color: white;
            background: crimson;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            text-decoration: none;
            box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.2);
            transition: 0.3s ease-in-out;
        }

        .btn:hover {
            background: darkred;
            transform: scale(1.1);
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.3);
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Ghada Ben Nasr</h1>
        <p>You are my heart, my soul, and my everything.</p>
        <p>Will you make me the happiest man alive?</p>
        <button class="btn" onclick="handleResponse('yes')">Yes</button>
        <button class="btn" onclick="handleResponse('no')">No</button>
    </div>

    <script>
        function handleResponse(answer) {
            if (answer === 'yes') {
                // Redirect to a "Yes" page or show a message
                window.location.href = 'yes.html'; // Replace with your actual "Yes" page URL
            } else {
                // Redirect to a "No" page or show a message
                window.location.href = 'no.html'; // Replace with your actual "No" page URL
            }
        }
    </script>
</body>
</html>
