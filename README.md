# TFM

Aqui van los cuadernos de Azure Databricks y archivos de datos utilizados.
En las subcarpetas se pueden encontrar el Pipeline de orquestacion, los cuadernos de generacion de datos falsos, y visualizacion del modelo de Favorabilidad

El video del proyecto puede verse en Youtube aquí: https://youtu.be/vaUej5PeWeg

## Credenciales / Credentials

Esta versión del repositorio no contiene credenciales. Los valores de acceso se reemplazaron por marcadores que deben completarse con los propios antes de ejecutar los cuadernos:

| Marcador | Dónde se usa |
|---|---|
| `<AZURE_STORAGE_KEY>` | Claves de las cuentas de Azure Data Lake Storage |
| `<PASSWORD>` | Contraseña de MongoDB Atlas y de Azure SQL Database |
| `<KAFKA_API_KEY>` / `<KAFKA_API_SECRET>` | Credenciales de Confluent Cloud (Kafka) |
| `<GOOGLE_API_KEY>` | Clave de API de Google (cuaderno de datos sintéticos) |

En Azure Databricks se recomienda guardarlas en un *secret scope* y leerlas con `dbutils.secrets.get(scope, key)` en lugar de escribirlas en el código.

This version of the repository contains no credentials. Access values were replaced with the placeholders above; supply your own (preferably through a Databricks secret scope) before running the notebooks.
