# Racing-Reward-
Claim your racing reward here dudes 😄
<!DOCTYPE html>
<html>
<head>
    <title>🎉 Congratulation! 🎉</title>
    <script>
        function startCountdown() {
            let count = 10;
            const countdown = setInterval(() => {
                document.getElementById("timer").textContent = count;
                count--;
                if (count < 0) {
                    clearInterval(countdown);
                    document.getElementById("reward-screen").style.display = "block";
                    document.getElementById("countdown").style.display = "none";
                }
            }, 1000);
        }

        function claimReward() {
            document.getElementById("reward-screen").innerHTML = `
                <h2>🏆 YOUR REWARD 🏆</h2>
                <div style="font-size: 24px">
                    <p>1 FREE hug from Mom</p>
                    <p>🦄 +5 Internet Points</p>
                    <p>🍕 Eternal Pizza Debt</p>
                </div>
                <p style="color: red">ERROR: Physical rewards expired in 1998</p>
                <button onclick="window.location.reload()">TRY AGAIN? 😅</button>
            `;
        }
    </script>
    <style>
        body { 
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        #countdown {
            font-size: 80px;
            margin: 30px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        button {
            background: gold;
            border: none;
            padding: 15px 30px;
            font-size: 20px;
            border-radius: 25px;
            margin: 20px;
            cursor: pointer;
        }
        #reward-screen {
            display: none;
        }
    </style>
</head>
<body onload="startCountdown()">
    <div id="countdown">
        <h
