1. Pull newest version from git:
`git clone "https://github.com/vektorprogrammet/vektorprogrammet.git`

2. Start docker-compose:
`docker-compose up -d`

3. Install dependencies:

- `docker-compose exec php npm install`
- `docker-compose exec php  composer install`

4. Build assets
`docker-compose exec php npm run build`

5. (DEV) Create database
`docker-compose exec php npm run db:reload`
