# Criar monitoramento Web zabbix via api 

## Dependencies

- Python3.8
- zabbix_api

## Requirements
```
pip3 install -r requirements.txt
```
## Pattern:

# Como usar

No arquivo urls.csv insira as urls que serão monitoradas conforme abaixo

```
https://url.com
https://url2.com
https://url3.com
```

# Execução do script
```
python3 create_web.py http://x.x.x.x/ Admin "NOME-HOSTNAME"
```
Será solicitado a senha 

# Funcionamento do script

O script irá verificar se existe um grupo de host chamado "Monitoramento URL" caso não irá criar, essa variável pode ser modificada no script, cada url recebe seu aplication* e trigger a nível disaster em caso de falha maior que 3

*application para versões abaixo de 6.0

## License
GPLv3