# MentorBit-DHT11

## Descripción

Esta librería está específicamente diseñada para ser utilizada junto con el módulo **MentorBit DHT11**.

El **MentorBit DHT11** es un sensor de temperatura y humedad. Esta librería permite obtener las lecturas de temperatura y humedad de manera fácil y rápida desde el sensor.

Puedes encontrar nuestro Módulo MentorBit y mucho más material de electrónica y robótica en nuestra tienda oficial:  [https://digitalcodesign.com/shop](https://digitalcodesign.com/shop)

## Métodos Principales

- `MentorBitDHT11` → Constructor de la clase.
- `obtenerTemperatura` → Obtiene y devuelve el valor de temperatura leído por el sensor DHT11 (tipo **float**).
- `obtenerHumedad` → Obtiene y devuelve el valor de humedad leído por el sensor DHT11 (tipo **float**).

## Instalación

Para instalar esta librería, simplemente copia el archivo `MentorBitDHT11.h` y `MentorBitDHT11.cpp` en la carpeta `libraries` de tu entorno de desarrollo (por ejemplo, en el IDE de Arduino).

## Constructor

```cpp
MentorBitDHT11 miModuloDHT11(pin);
```

Donde pin es el puerto donde está conectado el DHT-11 para recibir la lectura.

### Parámetros

- `pin`: Pin donde está conectado el sensor DHT11 (por defecto es 0).

## Métodos

### `float obtenerTemperatura()`

Obtiene y devuelve el valor de temperatura leído por el sensor DHT11.

#### Ejemplo de uso

```cpp
float temperatura = dht.obtenerTemperatura();
```

### `float obtenerHumedad()`

Obtiene y devuelve el valor de humedad leído por el sensor DHT11.

#### Ejemplo de uso

```cpp
float humedad = dht.obtenerHumedad();
```
