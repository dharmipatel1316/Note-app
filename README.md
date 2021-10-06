# Note-app

Insructions

TODO: The application should allow you to create, edit, and delete delete notes. Notes will be save to the database. Notes will have a title, content, and created_at displayed on the front end.

1. Save the created notes in the database
2. Create the necessary table with Laravel migrations
3. Create all require restful routes to achieve the CRUD functionality
4. Create required Front End components to access the API you created
5. Authenticated user needs to be able to view all notes, create new notes, edit existing notes, and delete notes.
6. Create phpunit tests for the new feature

Docker installation instructions here: https://docs.docker.com/compose/install/

Copy Laravel environment file (While in project root)

cp .env.example .env
Copy Docker environment files

cd docker

cp env-example .env
Run docker containers

docker-compose up
Enter workspace container

docker-compose exec --user=laradock workspace bash
Install dependencies and build existing database

composer install
npm install
php artisan key:generate
php artisan migrate --seed
Build app

npm run watch
The application should now be available at http://localhost
