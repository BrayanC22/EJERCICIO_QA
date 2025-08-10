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

## Requisitos

Asegúrate de tener instalados los siguientes componentes antes de ejecutar el proyecto:

1. Python 3.13.6: Asegúrate de que Python esté instalado en tu máquina. Si no lo tienes, puedes descargarlo desde aquí (https://www.python.org/downloads/).
   - Ejecutar el cmd con el siguiente comando "python --version", con la finalidad de verificar que se haya instalado correctamente la version de python.

2. Visual Studio Code (VS Code): Recomendado como entorno de desarrollo para escribir y ejecutar el código.
   - Si no lo tienes instalado, descárgalo desde [Visual Studio Code]	(https://code.visualstudio.com/Download).

3. Selenium WebDriver: Necesario para la automatización de pruebas en el navegador.
   - Este proyecto utiliza **Selenium WebDriver** y **WebDriver Manager** para manejar los controladores de navegador automáticamente.


## Instalación de Dependencias

Para ejecutar el proyecto, debes seguir estos pasos:

    ### 1. Clonar el Repositorio desde GitHub


Primero, descarga el repositorio en tu máquina local a través del Link del repositorio: "https://github.com/BrayanC22/EJERCICIO_QA.git" O si tiene git instalado abrir cmd y ejecutar el siguiente comando en la ruta deseada.

	git clone https://github.com/BrayanC22/EJERCICIO_QA.git


## Instrucciones para la Ejecución

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/BrayanC22/EJERCICIO_QA.git
   ```


2. **Instala las dependencias necesarias:**

- Abrir el visual code y abrir el proyecto descargado para este ejercicio es: "PruebaQA_Selenium", luego pulsar las teclas "Control + ñ" para que se abra una terminal. 

- Luego ejecutar el siguiente comando "pip install -r requirements.txt"
	-- Selenium: Selenium es utilizado para automatizar las interacciones con el navegador. Si no lo tienes, se instalará con pip desde el archivo "requirements.txt" a través del siguiente comando.

   ```bash
   pip install -r requirements.txt
   ```


3. **Ejecuta el script de prueba E2E:**

   Ejecuta el script de automatización con el siguiente comando:

   ```bash
   python test_saucedemo.py
   ```

	Este comando ejecutará el flujo completo de la prueba automatizada, que incluye:
	* Iniciar sesión en el sitio web.
	* Agregar dos productos al carrito.
	* Proceder al checkout y completar la compra.
	* Verificar que el mensaje de confirmación de compra sea "THANK YOU FOR YOUR ORDER".


## Conclusiones

Durante la ejecución de la prueba, el flujo de compra se automatizó correctamente, superando los inconvenientes con las alertas emergentes de Google. Usamos modo incógnito para evitar que estas alertas interfirieran con el test. El flujo de compra fue ejecutado desde el login hasta la confirmación de compra exitosa, como se esperaba.

Este enfoque te permite tener un control completo sobre la automatización del flujo de compra de Saucedemo, lo que te ayudará a realizar pruebas consistentes en cualquier momento.
