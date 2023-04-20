# Configurações para o Airflow

Para o Airflow funcionar corretamente precisamos entrar dentro do container e instalar algumas blibliotecas, para isso é necessario executar os seguintes comandos:

Comando para entrar no bash do container airflow
```docker container exec -it airflow bash```

Comando para instalar as bibliotecas
```pip install pymysql xlrd openpyxl minio```

No Webserver será necessario adicionar as variaveis do datalake e do database para o funcionamento correto.

Após acessar o Airflow vá na opção de Admin > Variables e adicione as seguintes variaveis.

data_lake_login
data_lake_password
data_lake_server
database_login
database_name
database_password
database_server

Cada variavel terá o seu respectivo valor, como na imagem abaixo, 

![airflow-variaveis.png](https://github.com/PauloHenrique1993/projeto_recursos_humanos/blob/main/images/airflow-variaveis.png?raw=true)