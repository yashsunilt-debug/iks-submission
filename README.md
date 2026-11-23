# IKS Research Website

React + Express starter website. It deliberately has **no SQLite, better-sqlite3, node-gyp, or native database dependency**, so Windows does not need Visual Studio C++ build tools for npm install.

## Run on Windows
1. Install Node.js LTS from https://nodejs.org/ (then close and reopen your terminal).
2. Extract this ZIP to a folder and open that folder in VS Code.
3. Terminal → New Terminal, then run `npm install`.
4. Run `npm run dev` and open http://localhost:5173.
5. Keep the terminal open. Stop with Ctrl+C.

For production preview run `npm run build`, then `npm start`, and open http://localhost:4000.

## Content
The five articles are starter frameworks. Replace them with accurate details and citations from your IKS research PDFs. Initial content is in `server/index.js`. The article edit box saves to `server/data/content.json` locally.

## GitHub
Create an empty repository, then in this folder run:
`git init`
`git add .`
`git commit -m "Initial IKS website"`
`git branch -M main`
`git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git`
`git push -u origin main`

## Hosting
Use a Node.js web service. Build command: `npm install && npm run build`; start command: `npm start`. A persistent disk is needed if you want edits stored in the JSON file to survive server restarts. The included edit endpoint is for a local/student demo; add authentication before allowing public edits.
