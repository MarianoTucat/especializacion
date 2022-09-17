# Opciones de ejecución

## Docker

Teniendo docker instalado:

- Descargar este repo completa
- Ir a la raiz de la carpeta que contiene los archivos descargados
- ejecutar ```docker compose up```
- acceder a http://127.0.0.1:8888/
- la clave es `test`

## Colab, ngrok y dynamodb con java

- Instalar [ngrok](https://ngrok.com/)
- Ejecutar `ngrok http 8000`
- Descargar [dynamodb local](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html)
- Ejecutar `java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb` en la carpeta recientemente descargada
- Abrir los archivos de jupyter en colab y configurar el endpoint usando la url provista por ngrok

## Jupyter local y dynamodb con java

- Instalar jupyter `pip3 install jupyter`
- Instalar boto3 `pip3 install boto3`
- Descargar [dynamodb local](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html)
- Ejecutar `java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb` en la carpeta recientemente descargada
- Ejecutar jupyter notebooks `jupyter notebooks`


