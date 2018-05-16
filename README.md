ASP.NET CORE + DOCKER

ASP.NET Core

ASP.NET Core es un marco multiplataforma de código abierto y de alto rendimiento que tiene como finalidad compilar modernas aplicaciones conectadas a Internet y basadas en la nube. Con ASP.NET Core puede hacer lo siguiente: Compilar servicios y aplicaciones web, aplicaciones de IoT y back-ends móviles. Usar sus herramientas de desarrollo favoritas en Windows, macOS y Linux. Efectuar implementaciones locales y en la nube. Ejecutarlo en .NET Core o en .NET Framework.

.NET CORE es una implementacion de codigo abierto, lo cual permite mayor transparencia y una comunidad activa, nos permite la ejecución mediante línea de comandos.

Mas informacion > https://docs.microsoft.com/es-es/aspnet/core/?view=aspnetcore-2.0

DOCKER

Anteriormente para realizar entornos de prueba, se corrían máquinas virtuales, las cuales como su nombre lo indica, montaban una máquina, con su sistema operativo, sus librerías y todo lo necesario para ejecutar la aplicación que deseamos, ejemplo un LAMP / WAMP, esto precisaba una gran cantidad de recursos físicos de la computadora que aloje la máquina virtual. Mediante Docker se logró optimizar esto solo utilizando el HOST y añadiendo las librerías necesarias para que la aplicación corra, esto permite agilizar la ejecución de la misma y la optimiza utilización de recursos, además posee una comunidad con proyectos estables que nos permiten descargar entornos de prueba para las diferentes necesidad, como nosotros descargamos un entorno con ASP.NET CORE para poder compilar el código que desarrollemos en cualquier editor/IDE

Como podemos instalarlo

Docker tiene un gran soporte sobre diferentes sistemas operativos.

Windows: La instalacion de Docker es como otras aplicaciones de la plataforma, descargando el .exe desde su web oficial (https://store.docker.com/editions/community/docker-ce-desktop-windows) y ejecutando el instalador.

Linux / Ubuntu

Se puede ingresar a la web https://get.docker.com/ Teniendo instalado “Curl” ejecutamos en consola $ curl -fsSL get.docker.com -o get-docker.sh $ sh get-docker.sh

MAC La instalacion de Docker es como otras aplicaciones de la plataforma, descargandolo desde su web oficial (https://store.docker.com/editions/community/docker-ce-desktop-mac) y ejecutando el instalador.

De esta forma tendrás instalado docker en tu sistema operativo. Luego con un comando podemos descargar contenedor que posee todo lo necesario para comenzar a trabajar con netcore Con estos comandos podremos correr nuestro ejemplo de aplicación web. “docker pull microsoft/dotnet” “docker run -it --rm -p 8000:80 --name aspnetcore_sample microsoft/dotnet-samples:aspnetapp”

Para mas informacion de como compilar y ejecutar desde un contenedor podemos observar https://hub.docker.com/r/microsoft/aspnetcore-build/

REFERENCIAS: ASP.NET CORE https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-2.0

DOCKER https://www.docker.com/get-docker

NET https://www.microsoft.com/net/download/

