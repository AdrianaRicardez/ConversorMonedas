# ConversorMonedas
Change ConversorMonedas Alura Latam

Este es un programa sencillo en Java que permite convertir cantidades entre diversas monedas utilizando las tasas de cambio proporcionadas por una API externa.

## Estructura del Proyecto

El proyecto está organizado en las siguientes clases:

1. **ApiClient**: Maneja las solicitudes a la API de tasas de cambio y procesa las respuestas.
2. **ApiResponse**: Modelo que representa la respuesta de la API, incluye las tasas de cambio y la última hora de actualización.
3. **Main**: Contiene el método principal que gestiona la lógica del conversor de divisas.
4. **Menu**: Ofrece métodos para mostrar el menú al usuario y seleccionar las monedas.

## Dependencias

- [Gson](https://github.com/google/gson) para el manejo de JSON.

## Instalación

1. Clona este repositorio.
2. Asegúrate de tener [Java 11](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) o superior instalado.
3. Importa el proyecto en tu IDE de preferencia.

## Uso

1. Ejecuta la clase `Main`.
2. Sigue las instrucciones en el menú para seleccionar la moneda base, la moneda objetivo, y la cantidad a convertir.

### Ejemplo de Uso

```bash
Bienvenidos al conversor de divisas
*******************************************
Seleccione una opción:
1) Convertir moneda
2) Salir

Ingrese su opción: 1

Seleccione la moneda base:
1) ARS - Peso argentino
2) BOB - Boliviano boliviano
3) BRL - Real brasileño
4) CLP - Peso chileno
5) COP - Peso colombiano
6) USD - Dólar estadounidense

Ingrese su opción: 6

Seleccione la moneda objetivo:
1) ARS - Peso argentino
2) BOB - Boliviano boliviano
3) BRL - Real brasileño
4) CLP - Peso chileno
5) COP - Peso colombiano
6) USD - Dólar estadounidense

Ingrese su opción: 1

¿Cuánto USD quiere convertir? 100

El cambio de 100.00 USD es 9420.00 ARS
Última actualización de la tasa de cambio: Sat, 10 Jul 2024 00:00:00 +0000

API de Tasas de Cambio
Este proyecto utiliza la API de ExchangeRate-API para obtener las tasas de cambio. Asegúrate de reemplazar la clave de API en ApiClient con tu propia clave:

private static final String API_URL = "https://v6.exchangerate-api.com/v6/TU_API_KEY/latest/";
