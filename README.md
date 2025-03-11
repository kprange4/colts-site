# Colt's Canine Club

## Initial Setup
1. Create a new branch to keep this "starter" clean.
2. Review and update the docker-compose file. Make sure to change the database volume for each different site.
3. Create environment file and update variables.
    ```shell
   cp .env.example .env
    ```
4. Execute the docker-compose.yml the .env file:
   ```shell
   docker compose up -d
   ```
5. Setup WordPress @ <http://localhost/>

## Update local environment files (Do this before making changes)
```shell
git checkout develop
git merge [your-branch]
git checkout [your-branch]
```

## Start running docker environment
```shell
docker compose up -d
```

### WordPress
<http://localhost>

### phpMyAdmin
<http://localhost:8081>

### MailHog
<http://localhost:8025>

## Update GitHub
This is on your branch:
```shell
git add -u *
git commit -m "[your-message]"
git push origin [your-branch]
git checkout develop
```
This is on develop branch:
```shell
git merge [your branch]
git push origin develop
```
