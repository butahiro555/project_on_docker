1. $ git clone https://github.com/butahiro555/docker_project.git
2. $ cd project_on_docker
3. $ mv .env.example .env
4. Setting your parameter on .env
5. $ cd docker/mysql
6. $ mv my.cnf.example my.cnf
7. Setting your parameter on my.cnf
8. $ cd ../..
9. $ docker compose up -d
10. $ docker compose exec -it app bash
11. $ composer create-project --prefer-dist laravel/laravel . "10.*"  #Laravelのバージョンは任意で決定
12. $ chmod -R guo+w storage
13. $ php artisan storage:link
14. Link the parameters mysql_parameter in docker_project/.env and DB_parameter in laravel/.env.
15. $ php artisan migrate
