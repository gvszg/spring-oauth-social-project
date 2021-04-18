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
### Github
OAUTH2_GITHUB_CLIENTID=<github-oauth-clientid>
OAUTH2_GITHUB_CLIENTSECRET=<github-oauth-clientsecret>

### Google
OAUTH2_GOOGLE_CLIENTID=<google-oauth-clientid>
OAUTH2_GOOGLE_CLIENTSECRET=<google-oauth-clientsecret>

### Facebook
OAUTH2_FACEBOOK_CLIENTID=<facebook-oauth-clientid>
OAUTH2_FACEBOOK_CLIENTSECRET=<facebook-oauth-clientsecret>
```

* Run spring-social

```bash
mvn spring-boot:run
```