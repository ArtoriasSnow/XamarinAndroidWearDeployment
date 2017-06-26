![alt text](https://www.blueboltsolutions.com/Portals/0/ContentImages/Logos/Xamarin%20Logo.png)
# Xamarin + Android Wear Emulator Deployment
Cómo desplegar (sin morir en el intento) una app utilizando un teléfono real y un emulador Wear Android (reloj)


Para este tutorial necesitaremos:

* Un teléfono Android real
* Un emulador Android Wear (creado desde el _Google Emulator Manager_)


Pasos a seguir:

1. Conectar teléfono al PC con el **modo depuración USB** activado
2. Instalar en teléfono la **App Android Wear** desde Google Play
3. Iniciar el emulador de Android Wear
4. Abrir terminal **SDK Command Prompt** (menú Tools) y escribir adb -d forward tcp:5601 tcp:5601
5. Abrir la app de Android Wear de nuestro teléfono y en el icono de configuración emparejar con el dispositivos Android Wear

# Solución al problema de Google Play Services

Utilizar la versión 42.1001.0 para todos los paquetes Xamarin.GooglePlayServices dado que existe un bug que impide la correcta comunicación entre el Wear emulador y el dispositivo móvil porque Xamarin detecta versiones incompatibles.

