First: git init
Type: git add .
Then: git commit -am "commit message"
Finally: git push

To push to Heroku
First: npm init (creates package.json)
Next: Edit package.json {
  Just above "test": type...
  "start": "node hello.js",
}
Then: add a new variable for the port {
  const PORT = process.env.PORT || 5000;
  modify .listen(PORT);
}
Then: Heroku login
Next: Heroku create
