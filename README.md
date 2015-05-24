Mecadopago bundle para Symfony2
============

Este bundle te permite adaptar de manera rápida el api de Mercadopago a tu proyecto en Symfony.

## License

### Version 0.1

### Things to know:

## Installation

**1**  Agrega en la llave `require` del composer.json

``` yml
    "require" : {
        "grunch/mercadopagobundle": "0.1",
    }
``` 

**2** Registra el bundle en ``app/AppKernel.php``

``` php
    $bundles = array(
        // ...
        new Grunch\MecardopagoBundle\GrunchMercadopagoBundle(),
    );
```

## Comienza

- Crea el objeto mercadopago:

``` php
$mp = $this->get('grunch_mercadopago');
```
- Crea las entidades con la consola :

``` bash
$ php app/console doctrine:schema:update --force
```
- Agrega tus credenciales de mercadopago:

``` yaml
# app/config/config.yml

grunch_mercadopago:
    client_id: xxxxxx
    client_secret: xxxxxxx
    sandbox: true
```
## Example

### More example

### For lazy devs

## Contributors

## Contribute

1. fork the project
2. clone the repo
3. get the coding standard fixer: `wget http://cs.sensiolabs.org/get/php-cs-fixer.phar`
4. before the PullRequest you should run the coding standard fixer with `php php-cs-fixer.phar fix -v .`

