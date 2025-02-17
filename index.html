<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wingspan Score Tracker</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Lora:wght@400;700&family=Quicksand:wght@400;600&display=swap');
        
        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #D7E8D4;
            color: #5C5346;
            padding: 20px;
            text-align: center;
        }
        h1, h2 {
            font-family: 'Lora', serif;
            color: #3E3B32;
        }
        .hidden { display: none; }
        button {
            background-color: #A7C4BC;
            color: white;
            border: none;
            padding: 10px 15px;
            margin: 10px;
            cursor: pointer;
            font-size: 16px;
            border-radius: 5px;
        }
        button:hover {
            background-color: #85A392;
        }
        input, select {
            padding: 8px;
            margin: 5px;
            border: 1px solid #B6A19E;
            border-radius: 5px;
            font-size: 16px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background-color: #F8F1EC;
        }
        th, td {
            border: 1px solid #B6A19E;
            padding: 10px;
            text-align: center;
        }
        th {
            background-color: #A7C4BC;
            color: white;
        }
    </style>
</head>
<body>
    <h1>Wingspan Score Tracker</h1>
    
    <div id="setup">
        <label for="numPlayers">Number of Players:</label>
        <input type="number" id="numPlayers" min="1" max="6">
        <button onclick="setupPlayers()">Next</button>
    </div>

    <div id="playerNames" class="hidden">
        <h2>Enter Player Names</h2>
        <div id="playerInputs"></div>
        <button onclick="setupGame()">Start Game</button>
    </div>

    <div id="scoreboard" class="hidden">
        <h2>Enter Scores</h2>
        <table>
            <thead>
                <tr id="scoreHeaders">
                    <th>Category</th>
                </tr>
            </thead>
            <tbody id="scoreBody">
                <!-- Score inputs will be added here dynamically -->
            </tbody>
        </table>
        <button onclick="calculateScores()">Calculate Scores</button>
        <h2 id="scores" class="hidden"></h2>
        <h2 id="winner" class="hidden"></h2>
    </div>

    <script>
        const categories = ["Birds", "Bonus Cards", "End-of-Round Goals", "Eggs", "Food on Cards", "Tucked Birds"];
        let players = [];
        
        function setupPlayers() {
            const numPlayers = document.getElementById("numPlayers").value;
            if (numPlayers < 1) return;
            
            const playerInputs = document.getElementById("playerInputs");
            playerInputs.innerHTML = '';
            
            for (let i = 1; i <= numPlayers; i++) {
                playerInputs.innerHTML += `<label>Player ${i} Name: <input type='text' id='player${i}'></label><br>`;
            }
            
            document.getElementById("setup").classList.add("hidden");
            document.getElementById("playerNames").classList.remove("hidden");
        }
        
        function setupGame() {
            players = [];
            const numPlayers = document.getElementById("numPlayers").value;
            for (let i = 1; i <= numPlayers; i++) {
                let playerName = document.getElementById(`player${i}`).value || `Player ${i}`;
                players.push(playerName);
            }
            
            const scoreHeaders = document.getElementById("scoreHeaders");
            const scoreBody = document.getElementById("scoreBody");
            scoreHeaders.innerHTML = '<th>Category</th>';
            scoreBody.innerHTML = '';
            
            players.forEach(player => {
                scoreHeaders.innerHTML += `<th>${player}</th>`;
            });
            
            categories.forEach(category => {
                let row = `<tr><td>${category}</td>`;
                players.forEach(() => {
                    row += `<td><input type='number' class='scoreInput' min='0'></td>`;
                });
                row += `</tr>`;
                scoreBody.innerHTML += row;
            });
            
            document.getElementById("playerNames").classList.add("hidden");
            document.getElementById("scoreboard").classList.remove("hidden");
        }
        
        function calculateScores() {
            let totals = players.map(() => 0);
            let scoreInputs = document.querySelectorAll(".scoreInput");
            let index = 0;
            
            categories.forEach((_, rowIndex) => {
                players.forEach((_, playerIndex) => {
                    totals[playerIndex] += parseInt(scoreInputs[index].value) || 0;
                    index++;
                });
            });
            
            let scoreText = "Scores:\n";
            players.forEach((player, i) => {
                scoreText += `${player}: ${totals[i]} points\n`;
            });
            
            document.getElementById("scores").textContent = scoreText;
            document.getElementById("scores").classList.remove("hidden");
            
            let maxScore = Math.max(...totals);
            let winners = players.filter((_, i) => totals[i] === maxScore);
            
            document.getElementById("winner").textContent = `Winner(s): ${winners.join(", ")} with ${maxScore} points!`;
            document.getElementById("winner").classList.remove("hidden");
        }
    </script>
</body>
</html>
