<div align = center>

# Práctica 3. Instalación de Windows Server 2022

<img src= "img/logo.JPG" width = "600">
</div>
<div align = right>

**Guillem Porta Ortuño**
</div>

---

## Requisitos del sistema
### Ejercicio 1: Requisitos de Windows Server 2022
**Accede a la web oficial de Microsoft y localiza los requisitos mínimos y recomendados de Windows Server 2022.**

<div align=center>
<img src = "img/cap1.png" width = "600">
</div>

| CPU          | RAM          |Almacenamiento| Red
|--------------|--------------|--------------|--------------|
| Procesador de 1,4 GHz de 64 bits|1 GB para Server Core| 32 GB de espacio|Un adaptador Ethernet que puede lograr un rendimiento de al menos 1 gigabit por segundo.|
| Compatible con el conjunto de instrucciones x64| 2 GB para servidor con experiencia de escritorio|  |  |

---

## Creación de la máquina virtual
### Ejercicio 2: Crea una nueva máquina virtual en VirtualBox con los parámetros adecuados. Configura la memoria, CPU y disco virtual justificando tus elecciones.
<div align=center>
<img src = "img/1.png" width = "600">
</div>

1. **Selección de la ISO y el nombre de la máquina:** 
En este primer apartado he introducido el nombre de la máquina tal y como indican las instrucciones del ejercicio (guiporort-ws2022), luego he añadido la ISO descargada anteriormente.
<div align=center>
<img src = "img/2.png" width = "600">
</div>

2. **Configuración de las especificaciones de la máquina:**
Luego, le he dado a la máquina 8GB (Más o menos) de memoria y 6 núcleos del procesador.
<div align=center>
<img src = "img/3.png" Width = "600">
</div>


3. **Montaje del almacenaniento:**
Por último, le he proporcionado 35GB de almacenamiento, ya que el mínimo requerido eran 32GB.

---

## Instalación de Windows Server 22
### Ejercicio 3: Documentación técnica.
**Antes de comenzar la instalación, crea un documento donde consten los datos más relevantes del proceso.**
|           Campo            |     Descripción    |
|----------------------------| -------------------|
| Sistema operativo          | Windows Server 2022|
| Fecha de instalación       | 05/11/2025         |
| Hora de inicio             | 16:10              |
| Hora de finalización       | 16:35              |
| Usuario administrador      | Administrador      |
| Contraseña                 | 79/gM:4581         |
| Ubicación de la VM         |   |
| Versión de VirtualBox      |   |
| Observaciones / incidencias|   |
### Ejercicio 4: Instalación de Windows Server 2022

<div align=center>
<img src="img/4.png" Width = "600">
</div>

1. **Selector de instalación**
Lo primero que he hecho al iniciar la instalación de la máquina es seleccionar que tipo de instalación voy a realizar. En este caso he seleccionado la segunda opción, que es la versión de Windows Server con interfaz gráfica o escritorio.
<div align=center>
<img src="img/5.png" Width = "600">
</div>

2. **Particionado de discos**
El segundo paso consiste en configurar el particionado de discos. La primera pantalla que nos aparece nos pregunta si queremos conservar los archivos existentes en el disco, o en su defecto borrar todos los existentes. Para esta instalación he seleccionado la segunda opción debido a que el disco sobre el que realizamos la instalación está vacío.
<div align=center>
<img src="img/6.png" Width = "600">
</div>
En el segundo apartado del particionado de discos debemos seleccionar como dividir los discos para la instalación, en este caso he realizado la partición más básica, que consiste en reservar el disco prácticamente entero como partición principal, separando únicamente 100MB para el sistema.
<div align=center>
<img src="img/7.png" Width = "600">
</div>

3. **Creación del usuario Administrador**
Por último, el instalador nos pide que le asignemos una contraseña al usuario principal, también conocido como administrador. Debido a las políticas de Windows Server 2022, nos obliga a insertar una contraseña considerablemente complicada, debido que no es una experiencia Windows de escritorio corriente y puede contener información sensible

<div align=center>
<img src="img/8.png" Width = "600">
</div>

4. **Comprobación de la instalación**
Lo primero que se suele hacer para comprobar que la instalación se ha realizado correctamente es iniciar sesión. Vemos que nos pide presionar la combinación de botones `"Ctrl + Alt + Supr"`, al estar usando una máquina virtual, necesitaremos añadir la tecla `"Ctrl derecho"` o en su defecto dirigirnos al botón "Entrada", "Teclado" y seleccionar `"Ctrl + Alt + Supr"`.

<div align=center>
<img src="img/9.png" Width = "600">
</div>

Aquí podemos observar que la instalación se ha realizado correctamente.

### Primeros pasos en Windows Server 2022
#### 1. Identifica el escritorio principal de Windows Server 2022 y localiza los siguientes elementos:
![Escritorio](img/Escritorio.png)

1. Menú de inicio:
2. Barra de tareas:
3. Área de notificación:
4. Acceso al Administrador del servidor (Server Manager).

#### 2. Explora el Administrador del servidor y revisa las secciones más importantes:

1. Dashboard o panel principal.
2. Local Server (información y configuración del servidor local).
3. All Servers (vista general de servidores).
4. Tools → inspecciona las herramientas disponibles.
5. Comprueba las opciones para añadir roles y características.
#### 3. Accede al Panel de control y a la aplicación Configuración para localizar opciones de:

1. Fecha y hora.
2. Región e idioma.
3. Red y adaptadores.
4. Programas y características.

#### 4. Abre el Administrador de tareas (Ctrl + Shift + Esc) y examina las pestañas principales:

1. Processes
2. Performance
3. Users
4. Services
#### 5. Consulta el Visor de eventos (eventvwr.msc) y localiza los registros más relevantes:

1. Application
2. Security
3. System