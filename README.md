# 🧵 Cimiento Textil SaaS
> *Construyendo lo que sigue: Transformación digital y operativa para la industria textil.*

---

## 🚀 1. Acerca del Proyecto (Problema y Propuesta de Valor)
*(Aquí respondes: ¿Qué problema resuelve?)*
- **El Problema:** Los pequeños y medianos talleres textiles sufren de pérdidas invisibles (mermas de tela no controladas), desorden en las órdenes de producción y hojas de cálculo obsoletas que generan errores en entregas.
- **La Solución:** CIMIENTO TEXTIL automatiza el flujo de trabajo desde la recepción de la orden hasta la entrega final, optimizando inventarios de rollos, avíos y trazabilidad de lotes.

---

## 🎯 2. Mercado Objetivo (¿Quién lo usará?)
*(Aquí respondes: ¿Qué tipo de negocio utilizará el sistema?)*
- Talleres de confección independientes.
- Micro y pequeñas empresas (PyMEs) textiles.
- Maquiladores que operan bajo demanda y necesitan control riguroso de tiempos y costos sin pagar licencias de ERPs corporativos complejos.

---

## 🛠️ 3. Stack Tecnológico
*(Aquí respondes: ¿Qué tecnologías planeas estudiar y utilizar?)*

| Capa / Módulo | Tecnología / Herramienta | Propósito en el SaaS |
| :--- | :--- | :--- |
| **Backend** | Java / Spring Boot | Microservicios, lógica de negocio y APIs REST |
| **Frontend** | Android / XML (Kotlin) | Interfaz móvil para operarios y supervisores |
| **Base de Datos** | PostgreSQL / MySQL | Persistencia transaccional con seguridad de datos |
| **Seguridad** | JWT (JSON Web Tokens) | Autenticación y control de accesos por roles |

---

## 🎯 4. Alcance del MVP (Objetivo de la Versión 1)
*(Aquí respondes: ¿Cuál es el objetivo de la primera versión?)*
- Validar el núcleo transaccional en un entorno real de taller.
- Permitir el registro de órdenes de producción básicas.
- Asignación de materias primas sin fricción ni errores humanos en el cálculo de insumos.

---

## 🔒 5. Arquitectura y Principio de Aislamiento (Multi-tenancy)
*(Aquí respondes: ¿Qué principio debe respetarse al separar los datos?)*
- **Aislamiento Estricto de Datos (Data Isolation):** Bajo ninguna circunstancia un taller (`tenant_a`) puede visualizar los inventarios, costos o clientes de otro taller (`tenant_b`). 
- **Implementación técnica:** Uso obligatorio de un filtro por `tenant_id` en las consultas a la base de datos respaldado por validaciones en el token de seguridad del backend.

---