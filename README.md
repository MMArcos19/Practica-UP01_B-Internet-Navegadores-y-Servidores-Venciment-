# Practica-UP01_B-Internet-Navegadores-y-Servidores-Venciment-
wordpress

2. Tecnologías utilizadas

Ubuntu: sistema operativo

Apache2: servidor web

MariaDB: base de datos

PHP: lenguaje necesario para WordPress

WordPress: gestor de contenidos

WooCommerce: gestión de la tienda online

GitHub: documentación y entrega del proyecto

3. Instalación

Para preparar el servidor se utilizan los siguientes comandos:

Actualizar el sistema:

sudo apt update
sudo apt upgrade -y

Instalar Apache:

sudo apt install apache2 -y
sudo systemctl enable --now apache2

Instalar MariaDB:

sudo apt install mariadb-server -y
sudo systemctl enable --now mariadb

Instalar PHP:

sudo apt install php libapache2-mod-php php-mysql php-curl php-gd php-mbstring php-xml php-zip php-intl php-bcmath unzip curl -y

4. Configuración de WordPress

Se instalará WordPress y se configurará para funcionar mediante un dominio local.

Nombre de la web: TecnoShop.

Dominio local: tecnoshop.local.

Panel de administración: tecnoshop.local/wp-admin.

5. Funcionalidades de la página web

La página web contará con las siguientes características:

Usuarios: tres cuentas con diferentes permisos.

Diseño: tema Astra personalizado.

Inicio de sesión: formulario para acceder a las cuentas.

Tienda online: WooCommerce.

Mapa: OpenStreetMap integrado en la página de contacto.

Chat: sistema de chat mediante Tawk.to.

Categorías: ordenadores, periféricos, componentes y accesorios.

Productos: diferentes artículos tecnológicos.

Reseñas: valoraciones de los productos.

Método de pago: transferencia bancaria de prueba.

Envíos: precio fijo, envío gratuito y recogida local.

6. Comprobación del servidor

Para comprobar que los servicios funcionan correctamente se utilizan estos comandos:

sudo systemctl is-active apache2
sudo systemctl is-active mariadb
php -v
curl -I http://tecnoshop.local
