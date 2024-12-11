<h2>Sistema de inventario, alertas, ticketing y restauración de imágenes con GLPI:</h2>

El proyecto consiste en implementar una herramienta de gestión de inventario, que en este caso será GLPI con varias funcionalidades añadidas. Este sistema esta diseñado para recopilar información sobre todos los equipos dentro de la red con la ayuda de OCS Inventory. También cuenta con un sistema de ticketing para recoger todas las incidencias que ocurran en los clientes.

Además de la gestión y monitoreo continuo de los equipos, contaremos con una herramienta para la implementación de un sistema de respaldo y restauración de imágenes en los ordenadores. Utilizaremos FOG Project, la cual puede implementar imágenes de disco por red utilizando el entorno de ejecución de prearranque. Esto asegurará la disponibilidad y la rápida recuperación de los datos en caso de fallos o incidentes, así como la rápida configuración de nuevos clientes. Separaremos los clientes por grupos, en este caso como si fuera una escuela de FP de informática (Profesor, DAM, DAW, ASIX…), y en función de esta clasificación, automatizar qué sistema operativo, softwares y configuraciones tendrá cada dispositivo.

Cada usuario contará con su propia carpeta personal en el servidor configurada con usuario y contraseña ya que al ser una escuela, los equipos estarán congelados y todo lo que no se guarde en la carpeta personal se borrará una vez se reinicie el equipo. Para esto configuraremos SambaAD para que cada usuario que quiera acceder a su carpeta tenga que introducir un usuario y una contraseña correcta.

Para fortalecer más la seguridad de la red, también utilizaremos una herramienta de análisis de vulnerabilidades automática. Utilizaremos Nessus, que proporciona escaneos automatizados de vulnerabilidades en los sistemas de la red, permitiendo la identificación automática de posibles debilidades en el software y la configuración de los equipos.



--------------------------------------------------------------------------------------------------

<h2>Inventory System with Alerts and Image Restoration using GLPI:</h2>

The project involves implementing an inventory management tool, which in this case will be GLPI with several added functionalities. This system is designed to gather information about all devices within the network with the help of OCS Inventory. It also includes a ticketing system to track and manage all incidents reported by users.

In addition to the continuous management and monitoring of devices, the project will include a tool for implementing a backup and image restoration system for computers. We will use FOG Project, which can deploy disk images over the network using the Preboot Execution Environment (PXE). This will ensure data availability and quick recovery in case of failures or incidents, as well as the rapid configuration of new devices. Clients will be organized into groups, in this case simulating an IT vocational training school (Teacher, DAM, DAW, ASIX…), and based on this classification, the operating system, software, and configurations for each device will be automated.

Each user will have their own personal folder on the server, protected by a username and password. Since this is a school setting, the devices will be frozen, meaning that anything not saved in the personal folder will be deleted upon reboot. To achieve this, we will configure SambaAD, ensuring that users must authenticate with a valid username and password to access their folders.

To further strengthen network security, we will also use an automatic vulnerability analysis tool. We will implement Nessus, which provides automated vulnerability scans on network systems, enabling the identification of potential weaknesses in software and device configurations.
