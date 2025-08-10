# README - Automatización E2E - Saucedemo

QA - Tester: Ing Brayan Calvopiña

Fecha: 8/09/2025

## Descripción del Proyecto

Este proyecto contiene la automatización del flujo de compra en la página https://www.saucedemo.com/. 

El flujo de trabajo incluye:

1. Autenticación con el usuario "standard_user" y la contraseña "secret_sauce".
2. Agregar dos productos al carrito.
3. Visualizar el carrito.
4. Completar el formulario de compra.
5. Finalizar la compra hasta la confirmación de "GRACIAS POR SU PEDIDO".

## Estructura del Proyecto

La estructura del proyecto es la siguiente:

```
/PruebaQA_Selenium
    ├── test_saucedemo.py         # Archivo principal que contiene el test automatizado
    ├── saucedemo.py              # Contiene la implementación de la clase Saucedemo para la automatización
    ├── config.py                 # Archivo para almacenar configuraciones como URL, usuario y contraseña
    ├── requirements.txt          # Archivo que contiene las dependencias del proyecto (Selenium, WebDriver Manager)
    ├── README.txt                # Este archivo con las instrucciones para ejecutar el proyecto
    ├── conclusiones.txt          # Conclusiones y hallazgos sobre la ejecución del proyecto
```

## Requisitos

Antes de ejecutar el proyecto, asegúrate de tener las siguientes herramientas y configuraciones:

1. **Python 3.13.6**:
   - **Verifica la instalación**: Ejecuta el siguiente comando en CMD:
     ```bash
     python --version
     ```
     Si no está instalado, descárgalo desde [python.org](https://www.python.org/downloads/).

2. **Visual Studio Code (VS Code)**:
   - Recomendado para desarrollar y ejecutar los scripts.
   - Puedes descargarlo desde [VS Code](https://code.visualstudio.com/Download).

3. **Selenium WebDriver** y **WebDriver Manager**:
   - Necesarios para automatizar las interacciones con el navegador. Se instalarán mediante el archivo `requirements.txt`.

## Instrucciones para la Ejecución

1. **Clona el repositorio:**

Para clonar el repositorio abrir un cmd en la ruta que desee clonar y ingrese el siguiente comando:

   ```bash
   git clone https://github.com/BrayanC22/EJERCICIO_QA.git
   ```
O si no tiene git instalado descarga el proyecto completo desde el repositorio.

```
	https://github.com/BrayanC22/EJERCICIO_QA.git
```

2. **Instala las dependencias necesarias:**

Abrir el visual code y abrir el proyecto descargado para este ejercicio es: "PruebaQA_Selenium".
  
Para instalar las dependencias necesarias, ejecuta el siguiente comando en la terminal de VS Code en caso de haberla cerrado abrirla con la combinación de teclas (Control + ñ):

```bash
pip install -r requirements.txt
```

Este comando instalará todas las librerías necesarias, como **Selenium** y **WebDriver Manager**.

## Instrucciones para la Ejecución

### 1. Ejecutar el Script de Prueba E2E

Una vez que hayas instalado todas las dependencias, puedes ejecutar el script de automatización con el siguiente comando en la terminal:

```bash
python test_saucedemo.py
```

Este comando ejecutará el flujo completo de la prueba automatizada, que incluye:
1. Iniciar sesión en el sitio web.
2. Agregar dos productos al carrito.
3. Proceder al checkout y completar la compra.
4. Verificar que el mensaje de confirmación de compra sea "THANK YOU FOR YOUR ORDER".


## Conclusiones

Durante la ejecución de la prueba, el flujo de compra se automatizó correctamente, superando los inconvenientes con las alertas emergentes de Google. Usamos modo incógnito para evitar que estas alertas interfirieran con el test. El flujo de compra fue ejecutado desde el login hasta la confirmación de compra exitosa, como se esperaba.

Este enfoque te permite tener un control completo sobre la automatización del flujo de compra de Saucedemo, lo que te ayudará a realizar pruebas consistentes en cualquier momento.
