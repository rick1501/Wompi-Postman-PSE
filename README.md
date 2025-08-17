# 🧪 Colección Postman – Wompi  

Esta colección valida la API de **Wompi (sandbox)** con pruebas de:  
- Consulta de **merchant** (válido e inválido).  
- Creación de **transacciones PSE** (exitosa, documento inválido, currency inválida).  

## ⚙️ Requisitos  
- Tener instalado **Postman**.  
- Llaves de prueba de Wompi (pública y privada).  
- Ambiente configurado con:  https://api.co.uat.wompi.dev/v1

  
## 🚀 Ejecución  
1. Importar el archivo `.json` de la colección en Postman.  
2. Configurar variables de entorno:  
 - `public_key`  
 - `private_key`  
 - `base_url`  
3. Ejecutar las pruebas manualmente o con **Runner**.  

## ✅ Resultados esperados  
- **200** → Merchant válido  
- **404** → Merchant inválido  
- **201** → Transacción PSE válida  
- **422** → Documento inválido  
- **Error** → Currency inválida  

---

👤 **Ricardo Narváez Contreras**  
QA Automation Engineer  

