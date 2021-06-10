# LaravelMiniProjetEmploisDeTemps
Mini-projet de gestionnaire d'emplois de temps : Laravel + Bootstrap + Css

Etape 1 : Installer les dépendances 
# cd dans le répertoire du projet
composer install
composer dumpautoload -o

Etape 2 : Vérifier que les valeurs de config/app.php sont les bonnes pour votre environnement
# Environment
'env' => env('APP_ENV', 'production'),
# Debug mode
'debug' => env('APP_DEBUG', false),
# URL
'url' => env('APP_URL', 'http://localhost'),

Etape 3 : Définir le fichier d'environnement à la racine du projet 
# Copier le template d'environnement
cp .env.example .env

Etape 4 : Générer la clé
php artisan key:generate

Etape 5 : Configuer le .env en fonction des besoins
(APP_*, DB_*, …)

Etape 5 :
php artisan config:clear
php artisan config:cache

Etape 6 : Connexion
php artisan serve
