#  Projet Minimalist-blog-laravel

## Si vous souhaitez utiliser le projet :

```bash
gitclone https://github.com/Choom87/Blog_Laravel.git
code .
```
## Créér un Alias pour l'utilisation de sail :
```bash
./vendor/bin/sail up -d
alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'
```


## Positionnez vous dans votre répertoire Projet et créer le fichier .env:

```bash
cd VotreRépertoireProjet
cp .env.example .env
```

```bash
docker run --rm --interactive --tty \
    --volume $PWD:/app \
    composer install
```
```bash
sail artisan key:generate    
sail artisan migrate
```

# Codage BDD - Migration des tables posts , Comment et Reply :

posts : 

```bash
sail php artisan make:model Post -mc     # migration et controller
```

Comment : 

```bash
sail php artisan make:model Comment -mc     # migration et controller
```
Reply :

```bash
 sail php artisan make:model Reply -mc     # migration et controller
```

# Implémentation de l'authentification (Laravel breeze) :

```bash
sail composer require laravel/breeze --dev

php artisan breeze:install
 
php artisan migrate
npm install
npm run dev
```
