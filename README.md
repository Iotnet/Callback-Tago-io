# Callback-Tago-io

Crear una cuenta en [Tago Io](https://admin.tago.io/signup)

Una vez entramos a nuestra cuenta, veremos el panel principal de Tago donde veremos cuantos recursos tenemos utilizados (devices, buckets, dashboards, etc), ya que al ser una cuenta gratuita, tendremos limitados varios recursos. Para la configuracion y creacion del dispositivo en Tago, iremos a la pestaña de DEVICES

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git1.png?raw=true)

seleccionaremos + ADD DEVICE

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git2.png?raw=true)

en la ventana que nos aparece, buscaremos Sigfox y seleccionaremos CUSTOM SIGFOX

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git3.png?raw=true)

escribiremos un nombre y en el DEVICE ID pondremos el ID de nuestro dispositivo. Dar clic en CREATE MY DEVICE (No poner ceros al inicio del ID)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git4.png?raw=true)

comenara a crear nuestro device y el bucket, donde se almacenaran los datos. Despues de unos segundos, terminara y seleccionaremos CONTINUE

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git5.png?raw=true)

daremos clic en GENERATE AUTHORIZATION

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git6.png?raw=true)

y nos mostrará una nueva ventana, donde debemos poner un nombre y selecionaremos GENERATE

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git7.png?raw=true)

enseguida ya tendremos generado nuestro token. Deberemos dar clic en COPY para copiar el token, el cual utilizaremos en la configuracion del callback en el backend de sigfox

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git8.png?raw=true)

Ingresamos a nuestra cuenta de backend

Deberemos configurar el callback con los siguientes datos:

      Type: DATA & UPLINK
      Channel: URL
      URL: https://sigfox.middleware.tago.io/uplink
      HTTP method: POST
      Headres:
          *Header*         *Value*
          device           {device}
          authorization    Token generado por TAGO
 
![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git9.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git10.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git11.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git12.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git13.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git14.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git15.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git16.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git17.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git18.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git19.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git20.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git21.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git22.png?raw=true)

![devkit_pinout](https://github.com/Iotnet/Callback-Tago-io/blob/main/images/tago_git23.png?raw=true)


