# Cars Importer

A docker wrapper to run services for an app which imports records from a CSV file.

## Setup

git clone git@github.com:enfie01s/csv-importer-docker.git --recursive

*If you didn't use the recursive flag when cloning, run this from inside the csv-importer-docker directory*
```git submodule update --init```

## Start the services and initial laravel installing
```
docker-compose build app
docker-compose up -d
docker-compose exec app composer install
docker-compose exec app php artisan key:generate
```

## Finally
In your browser, navigate to http://localhost
