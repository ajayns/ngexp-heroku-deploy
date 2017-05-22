# ngApp-Heroku

App to demostrate deploying an Angular Express WebApp into Heroku.

## Set up.
Make sure you have angular cli and heroku cli installed.
```bash
$ npm install -g angular-cli
$ npm install -g heroku
```

Clone the repo
```bash
$ git clone https://github.com/ajayns/ng2-mean.git
$ cd ng2-mean
```

Install dependencies
```bash
$ npm install
```

Test locally
```bash
$ ng build && node server.js
```

Configure Heroku
```bash
$ heroku login
$ heroku create <app-name>
```


Deploy the app, ensure one instance is running
```bash
$ git push heroku heroku:master
$ heroku ps:scale web=1
```

Open the app in browser from your heroku id or just type
```bash
$ heroku create
```