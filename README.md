# Digital-Clock
<!DOCTYPE html>
<html>
<head>
    <title>My Digital Clock</title>
    <style>
        body { background: #2c3e50; color: #1abc9c; display: flex; justify-content: center; align-items: center; height: 100vh; font-family: 'Arial', sans-serif; }
        #clock { font-size: 60px; border: 5px solid #1abc9c; padding: 20px; border-radius: 15px; box-shadow: 0 0 20px rgba(26, 188, 156, 0.5); }
    </style>
</head>
<body>
    <div id="clock">00:00:00</div>

    <script>
        function updateClock() {
            const now = new Date();
            const time = now.toLocaleTimeString();
            document.getElementById('clock').innerText = time;
        }
        setInterval(updateClock, 1000);
        updateClock();
    </script>
</body>
</html>
