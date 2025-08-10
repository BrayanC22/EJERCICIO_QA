
# Cypress PetStore API Tests

Este proyecto tiene como objetivo ejecutar pruebas de integración usando **Cypress** en la **API de PetStore**. El proyecto valida las operaciones básicas de la API, como la creación de mascotas, la consulta de mascotas por ID, la actualización del estado de una mascota y la consulta de mascotas por estado.

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

### 1. Clonar el repositorio

Primero, necesitamos clonar el repositorio que contiene el proyecto de pruebas. Abre una terminal y ejecuta el siguiente comando:

```bash
git clone https://github.com/tu_usuario/petstore-api-tests.git
```

Reemplaza `tu_usuario` con tu nombre de usuario de GitHub. Si no tienes acceso al repositorio, debes **crear un fork** o tener acceso al mismo.

### 2. Navegar al directorio del proyecto

Después de clonar el repositorio, navega al directorio del proyecto:

```bash
cd petstore-api-tests
```

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

Esto abrirá el **Test Runner** de Cypress, donde podrás ver las pruebas disponibles y ejecutar cada una de ellas de manera interactiva.

- **Ejecutar en modo interactivo:** Cypress abrirá una ventana en el navegador donde podrás hacer clic en las pruebas para ver sus resultados en tiempo real.

### 6. Ejecutar las pruebas en modo headless (opcional)

Si prefieres ejecutar las pruebas en **modo headless** (sin interfaz gráfica), puedes usar el siguiente comando:

```bash
npx cypress run
```

Este comando ejecutará todas las pruebas de manera automática en segundo plano y mostrará los resultados directamente en la terminal.

---

## Estructura del Proyecto

Aquí te mostramos una descripción de los archivos y carpetas principales del proyecto:

```
/cypress
    /integration
        petstore.spec.js           # Archivo principal de las pruebas de la API de PetStore
    /fixtures
        example.json               # Archivo de datos de prueba, si es necesario
    /support
        commands.js                # Comandos personalizados de Cypress, si es necesario
    /plugins
        index.js                   # Configuración de plugins de Cypress, si es necesario
/cypress.json                     # Archivo de configuración principal de Cypress
/package.json                     # Dependencias y scripts del proyecto
README.md                         # Este archivo
```

---

## Información adicional

### Cómo agregar nuevas pruebas

Si deseas agregar nuevas pruebas a la API de PetStore:

1. Dirígete a la carpeta `/cypress/integration/`.
2. Crea un nuevo archivo `.spec.js` para tu prueba.
3. Escribe tus pruebas siguiendo el mismo formato que se usa en `petstore.spec.js`.

### Personalizar Cypress

Si necesitas personalizar la configuración de Cypress, puedes editar el archivo `cypress.json` o agregar comandos personalizados en `commands.js` dentro de la carpeta `/cypress/support/`.

### Actualización de dependencias

Para actualizar las dependencias del proyecto, puedes ejecutar:

```bash
npm update
```

---

## Contribuciones

Si deseas contribuir al proyecto, por favor sigue estos pasos:

1. Realiza un **fork** del repositorio.
2. Crea una nueva rama (`git checkout -b feature/mi-nueva-caracteristica`).
3. Realiza los cambios y haz commit (`git commit -am 'Añadir nueva característica'`).
4. Empuja los cambios (`git push origin feature/mi-nueva-caracteristica`).
5. Crea un **pull request** desde tu fork a la rama principal del repositorio.

---

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
