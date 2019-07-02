# Heroku-Node.js-Express-PostgreSQL

Coder - Wang Harry

# How to deploy node project to Heroku free ?

-Download 64-bit installer or "brew install heroku/brew/heroku"
-heroku login
-git clone https://github.com/funnyjerry/Heroku-Node.js-Express-PostgreSQL.git
-cd Heroku-Node.js-Express-PostgreSQL
-heroku create
-git push heroku master
-heroku ps:scale web=1
-heroku open

# View logs
-heroku logs --tail

# Define a Procfile
- node index.js

# Scale the app
-heroku ps
-heroku ps:scale web=0
-heroku ps:scale web=1

# Declare app dependencies
- package.json
 {
  "name": "node-js-getting-started",
  "version": "0.3.0",
  ...
  "engines": {
    "node": "8.11.1"
  },
  "dependencies": {
    "ejs": "^2.5.6",
    "express": "^4.15.2"
  },
  ...
}
-npm install

# Run the app locally
-heroku local web

# Push local changes
-npm install cool-ascii-faces
-heroku local

# Git
-git add .
-git commit -m "Add cool face API"
-git push heroku master
-heroku open cool



