
# Pre-requirement

## Heroku

### Heroku client

1. install git: https://git-scm.com/downloadsDownload
2. install heroku-cli: https://devcenter.heroku.com/articles/heroku-cli
3. heroku --version
4. heroku login

### Heroku App

1. Create heroku application: https://dashboard.heroku.com/apps 
2. New > Create app
   * App name: [app-name]
   * Choose a region: [us]

### Heroku postgres

1. Create heroku postgres database: https://data.heroku.com/
2. Create one > install Heroku Postgres > Submit Order Form
   * Add-on plan: [HobbyDev-Free]
   * App to provision to: [app-name]
3. Setting > View Credentials
4. Copy your credentials to config/secret.json

## Dbeaver

1. Download + install: https://dbeaver.io/
2. New Database Connection > PostgreSQL > Test Connection > Ok
   * Host: [your-credentials]
   * Database: [your-credentials]
   * Username: [your-credentials]
   * Password: [your-credentials]
3. Rename Database (F2): Heroku-Flask


## Deploy
1. heroku git:remote -a [app-name]
2. git add .
3. git commit -am "make it better"
4. git push heroku master