# Procesamiento de pagos con tarjeta a través de Checkout Bricks
[English](README.md) / [Português](README.pt.md)

## :computer: Tecnologías
- Java 11
- [Spring Boot](https://spring.io/projects/spring-boot) 2.5.4
- [Maven](https://maven.apache.org/) (dependency manager)

## 💡 Requisitos
- Java 8 o superior (sigue las instrucciones de descarga [aquí](https://java.com/es/download/help/download_options.html)).
- [Lee nuestras instrucciones](https://www.mercadopago.com/developers/es/docs/getting-started) sobre cómo crear una aplicación en el Panel de Desarrolladores de Mercado Pago para obtener la public key y el access token. Estas llaves te darán acceso a las API de Mercado Pago.

## :gear: Instalación
1. Clona el proyecto.
```bash
git clone https://github.com/mercadopago/card-payment-bricks-sample-java.git
```

2. Accede a la carpeta del proyecto.
```bash
cd card-payment-bricks-sample-java
```

3. Ejecuta el siguiente comando:

Linux / MacOS
```bash
./mvnw clean install
```

Windows
```bash
./mvnw.cmd clean install
```

## 🌟 Como ejecutar
1. Ejecuta el siguiente comando para iniciar la aplicación:

Linux / MacOS
```bash
./mvnw spring-boot:run -Dspring-boot.run.arguments="--mercado_pago_sample_public_key=YOUR_PUBLIC_KEY --mercado_pago_sample_access_token=YOUR_ACCESS_TOKEN"
``` 

Windows
```bash
./mvnw.cmd spring-boot:run -Dspring-boot.run.arguments="--mercado_pago_sample_public_key=YOUR_PUBLIC_KEY --mercado_pago_sample_access_token=YOUR_ACCESS_TOKEN"
``` 

2. Recuerda cambiar los valores de `YOUR_PUBLIC_KEY` y `YOUR_ACCESS_TOKEN` por las [credenciales](https://www.mercadopago.com/developers/panel) de su cuenta.

3. Accede a http://localhost:8080 en tu navegador.

### :test_tube: Pruebas
En nuestras [instrucciones de prueba](https://www.mercadopago.com/developers/es/docs/checkout-bricks/integration/integration-test) encontrarás **[tarjetas de crédito](https://www.mercadopago.com/developers/es/docs/checkout-bricks/additional-content/test-cards)** que se pueden utilizar para simular el pago de este ejemplo, junto con una guía sobre cómo crear **usuarios de prueba**.

## :handshake: Contribuyendo
Puedes contribuir a este proyecto informando problemas y bugs. Antes de abrir una contribución, lee nuestro [código de conducta](CODE_OF_CONDUCT.md).

## :bookmark: Licencia
MIT License. Copyright (c) 2021 - Mercado Pago <br/>
Para obtener más información, consulte el archivo [LICENSE](LICENSE).