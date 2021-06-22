# Create Laravel Project with React

## init Laravel Project & Migrate
```
curl -s https://laravel.build/example-app | bash
cd example-app
./vendor/bin/sail artisan migrate
```

## install Breeze
```
./vendor/bin/sail composer require laravel/breeze --dev
```

## install React (you can remove react for blade or replace to vue for Vue.js)
```
./vendor/bin/sail artisan breeze:install react
./vendor/bin/sail npm install
./vendor/bin/sail npm run dev
```

## memo for proxies
```
./vendor/bin/sail artisan vendor:publish --provider="Fideloper\Proxy\TrustedProxyServiceProvider"
```