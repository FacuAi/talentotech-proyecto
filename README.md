# talentotech-proyecto.

# 🧪 Proyecto de Automatización de Pruebas – UI & API

Este repositorio contiene un proyecto de **automatización de pruebas de UI y API** desarrollado en **Python**, utilizando **Pytest**, **Selenium WebDriver** y **Requests**. El sitio bajo prueba para UI es **SauceDemo**, mientras que para API se utiliza **Reqres**.

El objetivo del proyecto es demostrar buenas prácticas de automatización, una arquitectura escalable y una correcta gestión de reportes, logs y datos de prueba.

---

## 🎯 Objetivo del proyecto

* Automatizar pruebas funcionales de **UI** y **API**
* Aplicar el patrón **Page Object Model (POM)**
* Utilizar datos externos (CSV / JSON)
* Generar reportes HTML automáticos
* Implementar logging detallado de ejecución
* Capturar pantallas automáticamente en tests fallidos

---

## 🛠️ Tecnologías utilizadas

* Python 3.x
* Pytest
* Selenium WebDriver
* Requests
* Faker
* Logging
* CSV / JSON

---

## 📁 Estructura del proyecto

```
project-root/
│
├── datos/
│   ├── data_login.csv
│   └── productos.json
│
├── logs/
│   └── suite.log
│
├── reports/
│   └── screens/
│
├── pages/
│   └── (Page Objects)
│
├── tests/
│   ├── ui/
│   └── api/
│
├── run_test.py
├── reporte.html
└── README.md
```

---

## 📊 Reportes y logs

Durante la ejecución de las pruebas se generan automáticamente los siguientes artefactos:

### 📄 Reporte HTML

* Archivo: `reporte.html`
* Ubicación: carpeta raíz del proyecto
* Contenido:

  * Lista de tests ejecutados
  * Estado de cada prueba (pass / fail)
  * Duración de cada test
  * Capturas de pantalla de pruebas fallidas

### 🧾 Logs de ejecución

* Archivo: `logs/suite.log`
* Incluye información detallada de:

  * Inicio y fin de ejecución
  * Acciones realizadas
  * Errores y excepciones

### 📸 Capturas de pantalla

* Se generan automáticamente cuando un test falla
* Ubicación:

```
reports/screens/
```

---

## ▶️ Ejecución de las pruebas

Para ejecutar todas las pruebas del proyecto, utilizar el siguiente comando:

```bash
python -m run_test.py
```

---

## ✅ Casos de prueba incluidos

### UI Testing (SauceDemo)

* Login exitoso
* Login fallido
* Login exitoso y fallido utilizando Faker
* Validaciones de la página de inventario
* Validaciones de la página del carrito

### API Testing (Reqres)

* GET users
* POST create user
* DELETE user
* Validación de códigos de estado HTTP
* Validación de estructura y contenido de respuestas JSON

---

## 📦 Manejo de datos de prueba

Los datos de prueba se gestionan de forma externa para facilitar el mantenimiento y la escalabilidad:

* `data_login.csv`

  * Usuarios válidos e inválidos para pruebas de login

* `productos.json`

  * Datos de productos utilizados para validaciones en UI

---

## 🧩 Arquitectura

El proyecto está diseñado con una arquitectura modular y escalable:

* Separación clara entre tests, pages y datos
* Uso de Page Object Model para UI
* Configuración centralizada
* Fácil incorporación de nuevos casos de prueba

---

## 📌 Conclusión

Este proyecto proporciona una base sólida para la automatización de pruebas de **UI y API**, siguiendo buenas prácticas de la industria. La estructura permite escalar fácilmente, agregar nuevos tests y mantener el código limpio y reutilizable.

Es ideal como proyecto de práctica, entrega académica o portfolio para roles de **QA Automation / Testing**.
