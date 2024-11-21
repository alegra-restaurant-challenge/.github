# Sistema de Gestión de Órdenes de Restaurante

## Descripción

Este proyecto es la implementación de una prueba técnica de backend para **Alegra**. El objetivo principal es desarrollar un sistema de microservicios para gestionar el proceso de preparación de platos en un restaurante de manera eficiente, utilizando **Node.js**.

## Características

- **Microservicios**: El sistema está compuesto por varios microservicios independientes que se comunican de manera asincrónica. Cada microservicio se encarga de una parte específica del flujo, como la cocina, la bodega de alimentos, y el historial de órdenes.
  
- **Dockerización**: Todos los microservicios están dockerizados para facilitar su despliegue y ejecución en diferentes entornos.
  
- **Peticiones Masivas**: El sistema está diseñado para soportar peticiones masivas de órdenes de platos.

- **Integración Externa**: El sistema se comunica con una **API externa** para la compra de ingredientes faltantes en la bodega de alimentos.

- **Gestión de Ingredientes**: Los ingredientes se gestionan a nivel de microservicio, y se verifica su disponibilidad en la bodega antes de proceder con la preparación de los platos.

- **Interfaz Gráfica**: Aunque el reto se centra en el backend, se ha añadido una interfaz básica para permitir la visualización de órdenes, ingredientes, y recetas.

## Requisitos

- **Node.js** 16+
- **Docker**
- **Git**

## Estructura del Proyecto

Este proyecto está compuesto por varios microservicios que incluyen:

1. **Cocina**: Microservicio encargado de recibir las órdenes y seleccionar aleatoriamente una receta para preparar el plato.
2. **Bodega de Alimentos**: Microservicio encargado de gestionar la disponibilidad de ingredientes en la bodega, y de hacer compras externas si los ingredientes no están disponibles.
3. **API Externa**: Conexión con un servicio externo para comprar ingredientes faltantes en la bodega.
4. **Interfaz Gráfica**: Interfaz básica que permite al gerente del restaurante ver las órdenes, los ingredientes disponibles y las recetas.

