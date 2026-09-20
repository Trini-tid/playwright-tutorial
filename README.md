# playwright-tutorial

# Playwright Tutorial 🎭

Este repositorio contiene una guía práctica y la configuración inicial para aprender a utilizar **Playwright** con **Node.js** para la automatización de pruebas de software y web scraping.

---

## 🚀 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado en tu sistema:
* **Node.js** (Versión 18 o superior recomendada)
* **npm** (Viene integrado con Node.js)

---

## 🛠️ Instalación y Configuración

Sigue estos pasos para configurar Playwright en tu entorno local desde cero:

### 1. Inicializar el proyecto
Si estás empezando un proyecto nuevo, genera el archivo `package.json` ejecutando en tu terminal:
```bash
npm init -y
```

### 2. Instalar Playwright
Ejecuta el instalador oficial de Playwright. Este comando descargará las dependencias necesarias y configurará la estructura base:
```bash
npm init playwright@latest
```

Durante la instalación, la terminal te hará un par de preguntas. Te recomendamos responder lo siguiente:
* **TypeScript or JavaScript?** Selecciona tu preferencia (JavaScript/TypeScript).
* **Where to put your end-to-end tests?** Presiona `Enter` (por defecto creará la carpeta `tests`).
* **Add a GitHub Actions workflow?** Escribe `false` (puedes añadirlo más adelante si lo deseas).
* **Install Playwright browsers?** Escribe `true` (instalará las versiones limpias de Chromium, Firefox y WebKit).

---

### 3.Para actualizaciones:
```bash
npm install -D @playwright/test@latest
npx playwright install --with-deps
```

## 🧪 Ejecutar las Pruebas

El instalador incluye unos tests de ejemplo para que verifiques que todo funciona correctamente. Puedes correrlos con los siguientes comandos:

* **Ejecutar todos los tests (Modo silencioso):**
  ```bash
  npx playwright test
  ```

* **Ejecutar tests con la interfaz gráfica (UI Mode):**
  ```bash
  npx playwright test --ui
  ```

* **Ejecutar tests en modo "Headed" (Viendo el navegador abrirse):**
  ```bash
  npx playwright test --headed
  ```

* **Ver el reporte de la última ejecución:**
  ```bash
  npx playwright show-report
  ```

---

## 📂 Estructura del Proyecto

Una vez instalado, verás una estructura de archivos similar a esta:
* `playwright.config.js` o `.ts`: Archivo de configuración global de Playwright.
* `tests/`: Carpeta donde escribirás tus archivos de prueba (ej. `example.spec.js`).
* `tests-examples/`: Un test de ejemplo muy completo interactuando con una app de tareas.