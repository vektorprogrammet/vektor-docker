1. Pull newest version from git and put it in app folder:
`git clone "https://github.com/vektorprogrammet/vektorprogrammet.git" app`

2. Start docker-compose:
`docker-compose up -d`

3. Install dependencies:

- `docker-compose exec php npm install`
- `docker-compose exec php composer install`

4. Build assets
`docker-compose exec php npm run build`

5. (DEV) Create database
`docker-compose exec php npm run db:reload`

6. Fix permissions
`docker-compose exec php chmod -R 755 /var/www`
