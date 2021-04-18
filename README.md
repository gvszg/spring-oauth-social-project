# OAuth Social Login Project

## Backend Server Setup
* Create MySQL database

```sql
mysql> create database spring_social;
```

* Configure database username and password

```bash
### Set Environment Variable
DB_URL=<db-url>
DB_PORT=<db-port>
DB_USERNAME=<db-username>
DB_PASSWORD=<db_password>
```

* Specify OAuth2 Provider ClientId's and ClientSecrets

```bash
### Set Environment Variable
### Github
OAUTH2_GITHUB_CLIENTID=<github-oauth-clientid>
OAUTH2_GITHUB_CLIENTSECRET=<github-oauth-clientsecret>

### Google
OAUTH2_GOOGLE_CLIENTID=<google-oauth-clientid>
OAUTH2_GOOGLE_CLIENTSECRET=<google-oauth-clientsecret>

### Facebook
OAUTH2_FACEBOOK_CLIENTID=<facebook-oauth-clientid>
OAUTH2_FACEBOOK_CLIENTSECRET=<facebook-oauth-clientsecret>

APP_OAUTH2_AUTHORIZEDREDIRECTURIS=http://localhost:3000/oauth2/redirect
```

* JWT Configure

```bash
### Set Environment Variable
APP_AUTH_TOKENSECRET=926D96C90030DD58429D2751AC1BDBBC
APP_AUTH_TOKENEXPIRATIONMSEC=864000000
```

* Run spring-social

```bash
mvn spring-boot:run
```

## Frontend Server Setup

```bash
cd react-social-frontend
npm install && npm start
```
