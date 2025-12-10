# XO Game (Tic-Tac-Toe)

This is a small XO / Tic-Tac-Toe game built in React JS.  
It’s a simple 3x3 board where two players can play on the same screen.

---

## What this project does

- 3x3 Tic-Tac-Toe board
- Two players: **X** and **O**
- Shows whose turn it is
- Detects **winner** or **draw**
- Button to **reset** the game
- Basic responsive layout so it works on mobile and desktop

Nothing fancy, just a clean starting point for an XO game.

---

## Tech stack

- **React JS** (with hooks)
- **JavaScript (ES6)**
- Styling: normal CSS or Tailwind CSS (up to you)
- Bundler: Vite or Create React App (project can be set up with either)

---

## Folder structure (example)

```bash
xo-game-react/
├── src/
│   ├── components/
│   │   ├── Board.jsx        # 3x3 grid
│   │   ├── Square.jsx       # single cell
│   │   └── StatusBar.jsx    # current player / winner text
│   ├── utils/
│   │   └── calculateWinner.js
│   ├── App.jsx
│   ├── main.jsx
│   └── styles.css           # or Tailwind setup
├── public/
├── package.json
└── README.md
You can change the structure as you like, this is just one way to keep it organized.

Getting started
Clone the repo:

bash
Copy code
git clone https://github.com/your-username/xo-game-react.git
cd xo-game-react
Install dependencies:

bash
Copy code
npm install
# or
yarn
Run the dev server
If using Vite:

bash
Copy code
npm run dev
# or
yarn dev
If using Create React App:

bash
Copy code
npm start
# or
yarn start
Then open the URL shown in the terminal (usually http://localhost:3000 or http://localhost:5173).

How to play
The game starts with Player X.

Click on any empty square to place your symbol.

Players take turns until:

Someone gets 3 in a row (horizontal, vertical, or diagonal), or

All 9 squares are filled (draw).

Use the Reset button to start a new game.

Short note on the game logic
The board is stored as an array of 9 items:

js
Copy code
const [board, setBoard] = useState(Array(9).fill(null));
currentPlayer toggles between "X" and "O" after each valid move.

After every move, a helper function calculateWinner(board) checks if there is a winner.

If there is a winner or the board is full, the game stops until you reset it.

Things you can add later (ideas)
Single-player mode vs computer (basic AI or minimax)

Move history (go back to previous steps)

Better UI, animations, sounds

Dark / light theme

Online multiplayer (socket-based)
```
