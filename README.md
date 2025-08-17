📑 README – Colección Postman Wompi
📌 Descripción

Esta colección contiene pruebas automatizadas en Postman para validar la integración con la API de Wompi (sandbox).
Incluye consultas de merchants y creación de transacciones PSE, tanto en escenarios exitosos como alternos.

⚙️ Requisitos Previos

Tener instalado Postman (versión más reciente).

Contar con las llaves de prueba de Wompi (pública y privada).

Ambiente configurado en Postman con la URL base:

https://api.co.uat.wompi.dev/v1

📂 Contenido de la Colección

Merchant

Consulta exitosa de merchant

Consulta con llave inválida

Transacciones PSE

Creación exitosa de transacción PSE

Creación de transacción con documento inválido

Creación de transacción con currency inválida

🚀 Ejecución de Pruebas

Importar el archivo .json de la colección en Postman.

Seleccionar el ambiente de pruebas (sandbox).

Configurar las variables de entorno:

public_key → Llave pública de prueba

private_key → Llave privada de prueba

base_url → https://api.co.uat.wompi.dev/v1

Ejecutar los requests individualmente o correr toda la colección con Runner.

✅ Resultados Esperados

200 OK al consultar un merchant válido.

404 Not Found al consultar un merchant con llave inválida.

201 Created al crear transacción PSE válida (estado inicial PENDING/CREATED).

422 Unprocessable Entity al intentar crear transacción PSE con documento inválido.

Error indicando currency inválida si se usa una moneda diferente a COP.

👤 Autor

Ricardo Narváez Contreras
QA Automation Engineer
