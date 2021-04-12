# ReCaptcha

## Recursos

O módulo usa o [Google reCAPTCHA V2](https://www.google.com/recaptcha/intro/index.html) para evitar spam na sua loja Magento, atualmente são suportados os seguintes formulários:

- Contato
- Análise do produto
- Criar conta
- Enviar o produto para um amigo
- Login
- Recuperar senha

## Instalação

Extraia os arquivos na raiz da loja

## Desinstalação

### Arquivos
```bash
rm -rf ./app/code/community/Studioforty9
rm -rf ./app/design/frontend/base/default/layout/studioforty9_recaptcha.xml
rm -rf ./app/design/frontend/base/default/template/studioforty9
rm -rf ./app/etc/modules/Studioforty9_Recaptcha.xml
rm -rf ./app/locale/en_US/Studioforty9_Recaptcha.csv
rm -rf ./app/locale/pt_BR/Studioforty9_Recaptcha.csv
```

### Banco de Dados
```sql
DELETE FROM core_config_data WHERE path LIKE 'google/recaptcha/%';
DELETE FROM core_resource WHERE code = 'studioforty9_recaptcha_setup';
```

## Documentação

http://recaptcha.readme.io/docs/

## Extendendo o módulo para utilizar com seus formulários

https://recaptcha.readme.io/v1.5/docs/developers

## Contribua

[Contribua comigo](https://github.com/studioforty9/recaptcha/blob/master/CONTRIBUTING.md)

Contribua com o autor original(https://github.com/studioforty9/recaptcha/blob/master/CONTRIBUTING.md)

## Licença

BSD 3 Clause [Ver licença](https://github.com/fredpiuma/magento_recaptcha/blob/master/LICENCE)
