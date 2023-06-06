---
layout: base
title: Tic tac toe
---

<html>
<head>
  <title>Tic Tac Toe</title>
  <style>
    .board {
      display: flex;
      flex-wrap: wrap;
      width: 300px;
    }
    .cell {
      border: 1px solid black;
      width: 100px;
      height: 100px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 48px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Tic Tac Toe</h1>
  <div class="board">
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
  </div>

  <script>
    // Get all the cells on the board
    const cells = document.querySelectorAll('.cell');

    // Player X starts the game
    let currentPlayer = 'X';

    // Function to check if a player has won
    function checkWinner() {
      const winningCombinations = [
        [0, 1, 2],
        [3, 4, 5],
        [6, 7, 8],
        [0, 3, 6],
        [1, 4, 7],
        [2, 5, 8],
        [0, 4, 8],
        [2, 4, 6]
      ];

      for (let combination of winningCombinations) {
        const [a, b, c] = combination;
        if (
          cells[a].textContent === currentPlayer &&
          cells[b].textContent === currentPlayer &&
          cells[c].textContent === currentPlayer
        ) {
          return true;
        }
      }

      return false;
    }

    // Function to check if the game is a draw
    function checkDraw() {
      for (let cell of cells) {
        if (cell.textContent === '') {
          return false;
        }
      }
      return true;
    }

    // Function to handle a player's move
    function makeMove() {
      if (this.textContent === '') {
        this.textContent = currentPlayer;

        // Check if the current player has won
        if (checkWinner()) {
          alert('Player ' + currentPlayer + ' wins!');
          resetGame();
          return;
        }

        // Check if the game is a draw
        if (checkDraw()) {
          alert('It\'s a draw!');
          resetGame();
          return;
        }

        // Switch to the other player
        currentPlayer = (currentPlayer === 'X') ? 'O' : 'X';
      } else {
        alert('Invalid move!');
      }
    }

    // Function to reset the game
    function resetGame() {
      for (let cell of cells) {
        cell.textContent = '';
      }

      currentPlayer = 'X';
    }

    // Add event listeners to each cell
    for (let cell of cells) {
      cell.addEventListener('click', makeMove);
    }
  </script>
</body>
</html>
