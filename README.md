# 🎮 Casual Games

A collection of fun, touch-friendly two-player games you can enjoy on the same device — perfect for playing with your toddler, family or friends!

## Games Included

| Game | Players | Description |
|------|---------|-------------|
| ❌⭕ **Tic-Tac-Toe** | 2 | Three difficulty levels — Easy (3×3, 3-in-a-row), Medium (up to 30×20, 4-in-a-row), Hard (up to 40×30, 5-in-a-row). Board size is **auto-suggested based on your screen size** |
| 🔴⚫ **Checkers** | 2 | Traditional draughts – jump over opponents, kings can move both ways |
| 🟡🔴 **Connect Four** | 2 | Drop discs and be the first to line up 4 in a row |
| 🃏 **Memory Match** | 1–2 | Flip emoji cards to find matching pairs – great for toddlers! Multiple grid sizes |
| ⬜ **Dots & Boxes** | 2 | Draw lines to complete boxes and claim them – grid sizes from 3×3 to 6×6 |

## Features

- **Touch optimised** – large tap targets, works great on phones & tablets  
- **Screen-adaptive board sizes** – Tic-Tac-Toe detects your screen and suggests the best board dimensions per difficulty  
- **No AI** – all games are two-player on the same device  
- **Difficulty levels** – each game includes options to increase challenge  
- **Score tracking** – running scores across rounds  
- **Custom player names** – personalise each session  
- **Fully offline** – works after first page load, no backend needed  
- **No dependencies** – pure HTML/CSS/JS, nothing to install  

## Tic-Tac-Toe Difficulty Levels

| Level | Win condition | Board size (phone) | Board size (tablet) | Board size (desktop) |
|-------|--------------|-------------------|--------------------|--------------------|
| 😊 Easy   | 3 in a row | 3 × 3   | 3 × 3    | 3 × 3    |
| 🤔 Medium | 4 in a row | ~10 × 8 | ~20 × 13 | ~30 × 20 |
| 😤 Hard   | 5 in a row | ~15 × 10| ~28 × 18 | ~40 × 30 |

Board dimensions are calculated live from your screen size. The scrollable board lets you explore even the largest grids on any device.

## Live Demo

The site is deployed via GitHub Pages:  
👉 **https://nubianlachlan.github.io/casual-games/**

## Project Structure

```
casual-games/
├── index.html               # Landing page
├── css/
│   └── styles.css           # Shared styles
├── games/
│   ├── tictactoe/index.html
│   ├── checkers/index.html
│   ├── connect-four/index.html
│   ├── memory/index.html
│   └── dots-boxes/index.html
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Pages deployment
└── README.md
```

## Deployment Instructions

### GitHub Pages (recommended)

The repository ships with a ready-made GitHub Actions workflow that publishes the site automatically.

1. **Fork or clone** this repository to your own GitHub account.
2. Go to **Settings → Pages** in your repository.
3. Under *Source*, select **GitHub Actions** (not a branch).
4. Push any commit (or re-run the workflow from the *Actions* tab) — the site will be live at  
   `https://<your-username>.github.io/<repo-name>/`

The workflow file is `.github/workflows/deploy.yml` and requires no secrets or configuration.

### Run Locally

Because the project is plain HTML/JS/CSS you can open it directly in a browser:

```bash
# Clone the repo
git clone https://github.com/nubianlachlan/casual-games.git
cd casual-games

# Option A – open index.html directly
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# Option B – serve with Python (avoids any path issues)
python3 -m http.server 8080
# then visit http://localhost:8080
```

### Deploy to Netlify / Vercel

Both services support static sites with zero config:

- **Netlify** – drag-and-drop the project folder onto [app.netlify.com/drop](https://app.netlify.com/drop), or connect your GitHub repo.  
- **Vercel** – run `npx vercel` inside the project directory.

## How to Play

### Tic-Tac-Toe
Choose a **difficulty level** — the board size is suggested automatically for your screen.  
Easy is a classic 3×3 board. Medium gives you a large board where you need **4 in a row**. Hard is a massive board where you need **5 in a row** — takes real strategy!

### Checkers
Red moves **up**, Black moves **down**. Tap a piece to select it (green squares show valid moves).  
Capture opponent pieces by jumping over them. Multiple jumps in one turn are allowed!  
Reach the opposite end to become a **King 👑** – kings move in both directions.

### Connect Four
Players alternate dropping discs into columns. The first to get **4 in a row** (horizontal, vertical, or diagonal) wins.

### Memory Match
All cards start face-down. On your turn flip two cards; if they match you keep them and go again.  
The player with the most matched pairs when all cards are cleared **wins**.  
Choose between 4×3 (Easy) and 6×5 (Expert) grids.

### Dots & Boxes
Players take turns tapping between two adjacent dots to draw a line. Complete all four sides of a box to claim it (and go again!).  
The player with the most boxes when the grid is full **wins**.

## Contributing

Pull requests are welcome! Ideas for new games or improvements:

- 🎲 Snakes & Ladders  
- ♟ Chess (simplified)  
- 🃏 Snap / Go Fish  
- 🎯 Battleship  

## Licence

MIT – free to use, share, and modify.
