# AppClima
Proyecto desarrollado con Swift, usando Vapor, Mysql y SwiftUI. Esta aplicación muestra en detalle el clima de la ciudad que se introduzca en el buscador y recomienda un outfit de acuerdo a temperatura, viento y condiciones de lluvia.

En Package.swift se hace la definición de las dependencia a usar, revisa que tengas las mismas para poder ejecutar sin problemas el proyecto.

Docker-compose.yml contiene las operaciones de los servicios que se usan, la base de datos y la api.

Clona el repositorio para poder usarlo y ejecuta swift build para instalar las dependencias de Package, recuerda checar que estén completas.

En la raíz del proyecto crea tu .env y egenera tu propia API KEY en openweathermap, es gratuita, esa KEY la replazaras en el código en cada línea donde se declara, incluido el .env

Para ejecutar localmente -- swift run
Con docker .. docker-compose up -d y abre en tu navegador http://localhost:8080

El proyecto está dividido en carpetas
Sources contiene los Models, Controllers y Migrations y para las imagenes estás definidas en la carpeta Public /images/outfits cada imagen dividida en categoria de género y clima.

Ejemplo de prueba: https://5a72-192-141-247-104.ngrok-free.app/weather-outfit?city=Toluca&genero=hombre
Los parametros city y genero son modificables, city puede tomar el valor de cualquier ciudad y genero toma valor hombre/mujer 
