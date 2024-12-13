

# MentorBit-DHT11

Esta librería está construida por Digital Codesign para utilizar el sensor DHT11, principalmente diseñado para el kit educacional "MentorBit".

Puedes encontrar nuestro MentorBit y mucho más material de electrónica y robótica en nuestra tienda oficial:  [https://digitalcodesign.com/shop](https://digitalcodesign.com/shop)

## Modo de empleo

Una vez tengamos la librería instalada desde el Arduino IDE, tenemos que incluir la librería con la siguiente línea:

```cpp
#include <MentorBitDHT11.h>
```

### Constructor

Una vez incluida la librería, usamos el constructor para crear el objeto del sensor DHT11 y definimos el pin al que está conectado:

```cpp
MentorBitDHT11 dht11Sensor(PIN_SENSOR);
```

Siendo `PIN_SENSOR` el pin al que está conectado el sensor DHT11.

### Uso

Con el objeto `dht11Sensor` definido, podemos obtener la lectura de la temperatura utilizando la función `obtenerTemperatura()`, que devuelve el valor de la temperatura medida en grados Celsius:

```cpp
float temperatura = dht11Sensor.obtenerTemperatura();
```

Además, si deseas obtener la humedad medida por el sensor, puedes usar la función `obtenerHumedad()`:

```cpp
float humedad = dht11Sensor.obtenerHumedad();
```

### Configuración de puertos

Si deseas configurar puertos personalizados, puedes usar la función `configPort()` para asignar los pines y configuraciones de puertos que necesitas:

```cpp
dht11Sensor.configPort(port);
```

Donde `port` es un objeto de tipo `Port` que contiene las configuraciones necesarias.

### Atributos

- `PIN_SENSOR`: Define el pin del sensor DHT11.




