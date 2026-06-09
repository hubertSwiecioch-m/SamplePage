<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>User Agent Detector</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f7f6;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background-color: #ffffff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 600px;
            text-align: center;
        }
        h1 {
            color: #333;
            margin-bottom: 20px;
        }
        .ua-box {
            background-color: #f0f0f0;
            padding: 15px;
            border-left: 5px solid #007BFF;
            border-radius: 4px;
            font-family: monospace;
            word-break: break-all;
            color: #555;
            text-align: left;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Your Device Details</h1>
        <p>When you connected, your browser sent the following User Agent string:</p>
        <div id="user-agent" class="ua-box">Detecting...</div>
    </div>

    <script>
        // Use JavaScript to grab the user agent string
        const currentUserAgent = navigator.userAgent;
        
        // Display it in the HTML container
        document.getElementById('user-agent').textContent = currentUserAgent;
    </script>

</body>
</html>
