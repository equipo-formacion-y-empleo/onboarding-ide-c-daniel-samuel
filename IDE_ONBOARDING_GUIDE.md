# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: Daniel Hernandez Singuña  
**Fecha V0**: 20/09/25  
**Fecha V1**: 19/12/25  

---

## Visual Studio Code - Entorno Principal

Visual Studio Code es un editor de código multiplataforma que, mediante extensiones, permite trabajar como un IDE completo para múltiples lenguajes. En esta guía se documenta su uso como entorno principal de desarrollo.

### Instalación y Verificación

**Método de instalación:**  

Descarga desde la página oficial mediante navegador web.

---

**Proceso de instalación:**

- **Descarga:** Accede a la página oficial:
  
  ![Página oficial de VS Code](screenshots/image1.png)

  Haz clic en el botón correspondiente a tu sistema operativo:
  
  ![Descarga del instalador](screenshots/image2.png)

  Guarda el archivo `.exe`, `.deb`, `.rpm` o `.pkg` según corresponda.

- **Opciones del instalador:**  
  Durante la instalación selecciona:

  - **Agregar al PATH**
  - **Registrar como editor predeterminado**
  - **Habilitar Code en el menú contextual**
  - **Instalar para todos los usuarios** (si está disponible)

  ![Opciones del instalador](screenshots/image3.png)

Estas opciones permiten que VS Code pueda ejecutarse desde accesos directos, integrarse con archivos de código y ampliar las funciones del explorador del sistema.

---

- **Verificación:**  
  Una vez instalado:

  1. Abre VS Code desde el icono del escritorio o menú inicio.
  2. Verifica que la ventana inicial carga correctamente.
  3. Comprueba las rutas internas desde *Help → About*.

  ![VS Code abierto](screenshots/image4.png)
  ![About de VS Code](screenshots/image5.png)

---

### Uso Básico de VS Code

**Navegación y funcionalidades básicas:**
- Navegación por la interfaz
- Edición de código
- Uso de la paleta de comandos
- Gestión de archivos y carpetas

![Interfaz principal de VS Code](screenshots/image6.png)
![Explorador de archivos](screenshots/image7.png)
![Paleta de comandos](screenshots/image8.png)

---

### Personalización del Entorno

**Configuraciones aplicadas:**  

Se personalizó el entorno visual y funcional de VS Code para mejorar la legibilidad, productividad y comodidad durante el desarrollo.

![Settings generales](screenshots/image9.png)

---

**Temas e iconos:**  
Se instaló un tema oscuro y un paquete de iconos desde la sección de extensiones.

- Tema aplicado: One Dark Pro  
- Iconos: Material Icon Theme

![Tema visual](screenshots/image10.png)
![Iconos de archivos](screenshots/image11.png)

---

**Configuración de fuentes:**  
Se configuró una fuente monoespaciada adecuada para programación.

- Fuente: Fira Code  
- Ligaduras activadas

![Configuración de fuente](screenshots/image12.png)

---

**Atajos de teclado útiles:**

- Ctrl+/ para comentar o descomentar código  
- Ctrl+Shift+P para abrir la paleta de comandos  
- Ctrl+` para abrir la terminal integrada  
- Alt+↑/↓ para mover líneas de código  

![Atajos de teclado](screenshots/image13.png)

---

**Configuración del editor:**

- Formateo automático al guardar  
- Detección automática de indentación  
- Ajuste de líneas largas (word wrap)  

![Configuración del editor](screenshots/image14.png)

---

**Terminal integrada:**

- Terminal predeterminada configurada como PowerShell  
- Uso de la terminal integrada para mostrar salidas de ejecución  

![Terminal integrada](screenshots/image15.png)

---

### SDK .NET

**Proceso de instalación:**

1. **Descarga e instalación:**  
   Se descarga el SDK .NET desde la página oficial de Microsoft y se ejecuta el instalador con las opciones predeterminadas.

   ![Descarga SDK .NET](screenshots/image16.png)

2. **Verificación:**  
   VS Code reconoce automáticamente el SDK al crear un proyecto C#.

   ![SDK reconocido](screenshots/image17.png)

---

### Configuración para C#

**Extensiones esenciales:**
- **Soporte oficial para C#** (C# Dev Kit)

![Extensión C# instalada](screenshots/image18.png)

---

**Configuraciones específicas para C#:**  
Se habilitó IntelliSense, formateo automático y soporte de depuración integrado.

![Configuración C#](screenshots/image19.png)

---

**Debugging básico:**
- Uso de puntos de interrupción
- Ejecución con y sin depuración
- Inspección de variables

![Debugging C#](screenshots/image20.png)

---

### Flujo de Trabajo con C#

**Creación de proyectos:**

1. Abrir la paleta de comandos.
2. Seleccionar `.NET: New Project`.
3. Elegir **Console Application**.
4. Asignar nombre y ubicación al proyecto.

![Creación proyecto C#](screenshots/image21.png)

---

**Estructura de proyecto:**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hola mundo desde C# en VS Code");
    }
}

```
**Compilación y ejecución:**

El proceso de compilación y ejecución de proyectos C# en Visual Studio Code se realiza directamente desde el propio editor utilizando el SDK .NET instalado previamente.

1. Abre el proyecto C# en VS Code.
2. Verifica que el archivo `Program.cs` contiene el método `Main`.
3. Ejecuta el proyecto pulsando **Ctrl + F5** para ejecutar sin depuración.
4. La salida del programa se muestra en la terminal integrada.

![Compilación y ejecución C#](screenshots/image31.png)

---

**Debugging:**

La depuración permite analizar el comportamiento del programa durante su ejecución.

1. Coloca un breakpoint haciendo clic a la izquierda del número de línea.
2. Pulsa **F5** para iniciar la ejecución en modo depuración.
3. Observa el valor de las variables en el panel de depuración.
4. Usa los controles de continuar, paso a paso y detener ejecución.

![Debugging en C#](screenshots/image32.png)

---

## Visual Studio - IDE Alternativo

### Instalación

**Proceso de instalación:**

- **Descarga:** Dirígete a la página oficial de Visual Studio en (https://visualstudio.microsoft.com/es/) y descarga la versión Community, que es gratuita y suficiente para desarrollo en C#.

  ![click en descargas](screenshots/image33.png)

- **Componentes necesarios:**  
  Al abrir el instalador, selecciona la carga de trabajo **Desarrollo de escritorio con .NET**. Esta incluye todo lo necesario para crear y ejecutar aplicaciones en C#. Opcionalmente, puedes seleccionar **ASP.NET y desarrollo web** si planeas usar proyectos web más adelante.

  ![Componentes del instalador](screenshots/image34.png)

- **Verificación:**  
  Una vez finalizada la instalación, abre Visual Studio. En la ventana de inicio, haz clic en **Crear un nuevo proyecto** y verifica que aparece la opción **Aplicación de consola (.NET Core / .NET 6/7/8)**. Si aparece, la instalación se ha realizado correctamente.

  ![Verificación Visual Studio](screenshots/image35.png)

---

### Desarrollo con C#

**Creación de proyecto:**

1. Abre Visual Studio.
2. Selecciona **Crear un nuevo proyecto**.
3. Filtra por **C#** y selecciona **Aplicación de consola (.NET)**.
4. Asigna un nombre al proyecto y selecciona la ubicación.
5. Haz clic en **Crear**.

![Creación de proyecto en Visual Studio](screenshots/image36.png)

---

**Flujo de trabajo básico:**

- **Compilación y ejecución:**  
  Pulsa **Ctrl + F5** para ejecutar sin depurar o **F5** para ejecutar con depuración.

- **Uso de Solution Explorer:**  
  Permite navegar entre archivos del proyecto, referencias y dependencias.

- **Debugging básico:**  
  Se utilizan breakpoints y el panel de depuración para inspeccionar variables y controlar la ejecución.

![Flujo de trabajo Visual Studio](screenshots/image37.png)

---

## Configuración de Lenguaje Adicional

**Lenguaje seleccionado:** Python - **Justificación:** Lenguaje ampliamente usado para desarrollo rápido, scripting, ciencia de datos y automatización.

### Instalación del Entorno

**Runtime/SDK:**

- **Descarga e instalación:**

  - Dirígete a https://www.python.org/downloads/
  - Descarga la última versión estable.
  - Marca la opción **Add Python to PATH** durante la instalación.

  ![Instalación de Python](screenshots/image38.png)

- **Verificación:**

  - Abre una terminal y ejecuta:

        python --version

  - El sistema muestra la versión instalada correctamente.

  ![Verificación Python](screenshots/image39.png)

---

### Configuración en VS Code

**Extensiones por lenguaje:**

*Para Python:*

- **Python**: Incluye soporte completo de intérprete, linting, debugging y Jupyter Notebook.

![Extensión Python VS Code](screenshots/image40.png)

---

**Configuraciones específicas aplicadas:**

- Selección del intérprete: **Ctrl+Shift+P → Python: Select Interpreter**
- Activación de **Format On Save**
- Activación de **Pylint** para mejorar la calidad del código

![Configuración Python](screenshots/image41.png)

---

### Proyecto de Ejemplo ###

**Código desarrollado:**

![Código Python](screenshots/image42.png)

---

**Proceso de ejecución:**

1. Abre el archivo `HolaMundo.py` en Visual Studio Code.
2. Pulsa **F5** para ejecutar con debugging o **Ctrl+F5** para ejecutar sin debugging.
3. Observa la salida en la terminal integrada.

![Ejecución Python](screenshots/image43.png)

## Configuraciones Recomendadas

**Configuraciones generales:**
- Activar **Auto Save** desde *File → Auto Save*.
- Activar formateo automático al guardar desde *Settings → Editor: Format On Save*.
- Configurar un tema oscuro para reducir la fatiga visual.
- Ajustar el tamaño de fuente y el espaciado de tabulación según preferencia.

![Auto Save activado](screenshots/image44.png)
![Format On Save](screenshots/image45.png)

---

**Herramientas adicionales:**
- **Git** para control de versiones local.
- **GitHub** para alojamiento de repositorios y trabajo colaborativo.
- Extensiones de productividad como:
  - Prettier
  - GitLens
  - Bracket Pair Colorizer

![Extensiones adicionales](screenshots/image46.png)

---

**Solución de problemas comunes:**

- **Problema:** Visual Studio Code no detecta Python  
  **Solución:**  
  Abrir la paleta de comandos con **Ctrl+Shift+P**, seleccionar **Python: Select Interpreter** y elegir la ruta correcta del intérprete instalado.

![Selección de intérprete](screenshots/image47.png)

---

- **Problema:** Error al ejecutar C#  
  **Solución:**  
  Verificar que el SDK de .NET está instalado correctamente y que la extensión **C# Dev Kit** está habilitada en Visual Studio Code.

![Error C#](screenshots/image48.png)

---

**Recursos útiles:**
- [[Enlace](https://learn.microsoft.com/es-es/visualstudio/?view=vs-2022)]: Guía completa sobre instalación, configuración, depuración y desarrollo de proyectos en Visual Studio y Visual Studio Code.
- [[Documentación](https://learn.microsoft.com/es-es/python/)]: Documentación oficial de Python con ejemplos, librerías estándar y buenas prácticas.

---