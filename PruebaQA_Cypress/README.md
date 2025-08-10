# README - Cypress PetStore API Tests

QA - Tester: Ing Brayan Calvopiña

Fecha: 8/09/2025

# Descripción del Proyecto

Este proyecto tiene como objetivo ejecutar pruebas de integración usando **Cypress** en la **API de PetStore**. El proyecto valida las operaciones básicas de la API, como la creación de mascotas, la consulta de mascotas por ID, la actualización del estado de una mascota y la consulta de mascotas por estado.


## Estructura del Proyecto

Aquí te mostramos una descripción de los archivos y carpetas principales del proyecto:

```
/cypress
    /integration
        petstore.spec.js           # Archivo principal de las pruebas de la API de PetStore
    /fixtures
    /support
        commands.js                # Comandos personalizados de Cypress, si es necesario
    /plugins
        index.js                   # Configuración de plugins de Cypress, si es necesario
/cypress.config.js                 # Archivo de configuración principal de Cypress
/package.json                     # Dependencias y scripts del proyecto
README.md                         
```

## Requisitos previos

Antes de comenzar, asegúrate de tener instalado lo siguiente en tu máquina:

### 1. **Instalar Node.js**
   **Node.js** es necesario para ejecutar Cypress, ya que Cypress depende de este entorno de ejecución.

   - **¿Cómo instalarlo?**
     1. Dirígete a [la página de descargas de Node.js](https://nodejs.org/).
     2. Descarga la versión recomendada para la mayoría de los usuarios.
     3. Sigue las instrucciones del instalador. Esto instalará tanto **Node.js** como **npm** (el gestor de paquetes de Node).

   **Verifica la instalación de Node.js y npm:**
   Una vez que Node.js esté instalado, abre una terminal o línea de comandos y ejecuta:
   ```bash
   node -v
   npm -v
   ```
   Esto debería mostrar la versión de `Node.js` y `npm` instalados.

### 2. **Instalar Git**
   **Git** es necesario para clonar el repositorio desde GitHub.

   - **¿Cómo instalarlo?**
     1. Dirígete a [la página de Git](https://git-scm.com/).
     2. Descarga el instalador adecuado para tu sistema operativo.
     3. Sigue las instrucciones del instalador.

   **Verifica la instalación de Git:**
   Una vez que Git esté instalado, abre una terminal y ejecuta:
   ```bash
   git --version
   ```
   Esto debería mostrar la versión de Git instalada.

### 3. **Instalar Cypress**
   **Cypress** es una herramienta de testing de JavaScript que nos permite realizar pruebas en aplicaciones web. Lo instalaremos a través de npm.

   - **¿Cómo instalar Cypress?**
     No necesitas instalar Cypress globalmente en tu máquina. Lo instalaremos como parte del proyecto en los siguientes pasos.

---

## Pasos para ejecutar el proyecto

Ahora, sigue estos pasos para configurar y ejecutar las pruebas en Cypress en tu máquina, desde cero.

### 1. Clonar el repositorio o Descargar el proyecto

Primero, necesitamos clonar el repositorio que contiene el proyecto de pruebas. Abre una terminal y ejecuta el siguiente comando:

```bash
git clone https://github.com/BrayanC22/EJERCICIO_QA.git 
```
o si no cuentas con git, puedes descargar el proyecto directo desde el repositorio (https://github.com/BrayanC22/EJERCICIO_QA.git) y asi ejecutarlo de forma local, en este caso la "PruebaQA_Cypress". 

### 2. Navegar al directorio del proyecto

Después de clonar el repositorio, navega al directorio del proyecto:

```bash
cd PruebaQA_Cypress 
```
* Reemplaza la ruta del directorio donde se encuentra descargado el proyecto 
### 3. Instalar las dependencias

Ahora, necesitamos instalar las dependencias necesarias, que incluyen **Cypress** y otras herramientas. Ejecuta el siguiente comando en la terminal:

```bash
npm install
```

Este comando instalará todas las dependencias definidas en el archivo `package.json`, incluyendo **Cypress**.

### 4. Verificar la instalación de Cypress

Después de ejecutar `npm install`, verifica que Cypress esté correctamente instalado ejecutando el siguiente comando en la terminal:

```bash
npx cypress open
```

Este comando abrirá la interfaz gráfica de Cypress. Si todo está correctamente instalado, podrás ver las pruebas y ejecutar los tests en la ventana del navegador.

### 5. Ejecutar las pruebas

Ahora, ya puedes ejecutar las pruebas. Para hacerlo, simplemente ejecuta:

```bash
npx cypress open
```

Esto abrirá el **Test Runner** de Cypress, donde podrás ver las pruebas disponibles y ejecutar cada una de ellas de manera interactiva, en este caso encontrar en la pestaña de "run" del navegador que se abrio y encontraras un archivo ".spec.js" que tendra la ejecucion de pruebas y se podra validar su funcionamiento.


## Información adicional

### Cómo agregar nuevas pruebas

Si deseas agregar nuevas pruebas a la API de PetStore:

1. Dirígete a la carpeta `/cypress/integration/`.
2. Crea un nuevo archivo `.spec.js` para tu prueba.
3. Escribe tus pruebas siguiendo el mismo formato que se usa en `petstore.spec.js`.


### Actualización de dependencias de ser necesario (Opcional)

Para actualizar las dependencias del proyecto, puedes ejecutar:

```bash
npm update
```

## Conclusiones:

El proyecto está diseñado para ser flexible y escalable, permitiendo agregar nuevas pruebas o adaptar la estructura a otros casos de uso. el proceso de integración de Cypress fue fluido. La configuración fue sencilla, y las pruebas de creación, consulta, actualización y filtrado por estado de las mascotas fueron fáciles de escribir y ejecutar. La flexibilidad de Cypress permitió que el flujo de pruebas fuera claro y robusto, haciendo que el proyecto fuera escalable para agregar más pruebas en el futuro. En general, el uso de Cypress resultó ser una herramienta poderosa para validar la API, y aunque hubo pequeños desafíos técnicos, la solución fue rápida y eficiente, lo que permitió completar el proyecto exitosamente.
