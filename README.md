# ead_php_devmedia_hello-world-laravel

> Projeto referente a [este](https://www.devmedia.com.br/laravel-criando-um-hello-world/40676) e [este](https://www.devmedia.com.br/primeiros-passos-com-laravel/40687) [desse guia](https://www.devmedia.com.br/laravel/)

## Setup

- O PHP na versão 7.2 ou superior
- O Composer
- Um servidor como Apache/Nginx
- E um editor de código ou IDE de sua preferência
- As extensões BCMath, Ctype, JSON, XML, OpenSSL, PDO, Mbstring, Tokenizer precisam estar habilitadas. Para verificar ou habilitá-las é necessário editor o arquivo php.ini que se encontra na pasta de instalação do PHP.

```sh
# php -m
php -r "var_dump([
    extension_loaded('bcmath'),
    extension_loaded('ctype'),
    extension_loaded('json'),
    extension_loaded('xml'),
    extension_loaded('openssl'),
    extension_loaded('pdo'),
]);"
```

## Run

```sh
php artisan serve
```

## Explicações

### Criação desse projeto

```sh
composer create-project --prefer-dist laravel/laravel hello-world
```

### Diretórios

- **App** - código principal do seu aplicativo.
- **Bootstrap** - inicializa a estrutura (`app.php`).
- **Config** - configuração do seu aplicativo..
- **Database** - database migrations, model factories, and seeds.
- **Public** - ponto de entrada para todas as solicitações (`index.php`) que entram no seu aplicativo e configura o carregamento automático.
- **Resources** - visualizações e seus recursos brutos, não compilados, como LESS, SASS ou JavaScript.
- **Routes** - definições de rota (`web.php`, `api.php`, `console.php` e `channels.php`).
- **Storage** - modelos Blade compilados, sessões baseadas em arquivo, caches de arquivos e outros arquivos gerados pela estrutura.
- **Tests** - testes automatizados.
- **Vendor** - dependências do Composer.

### Componentes

- **Rotas** - Endereços para recursos.
- **Views** - Respostas devolvidas para o cliente.
- **Controllers** - Classes que contém a lógica para o tratamento das requisições. Podem ser criadas via cli com ``php artisan make:controller PrimeiroController``
- **Models** - Classes que contém regras de negócio. Podem ser criadas via cli com ``php artisan make:model PrimeiroModel``
