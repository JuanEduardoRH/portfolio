# Portafolio de Proyectos

## Índice

- [Sistema de Gestión para Restaurantes](#sistema-de-gestion-para-restaurantes)
- 
---

# Sistema de Gestión para Restaurantes

Este proyecto fue desarrollado con el objetivo de demostrar mis habilidades como desarrollador Full Stack, abordando la creación de un sistema integral para la gestión de un restaurante. La plataforma cubre áreas clave como la administración de mesas, la gestión de comandas en cocina y bar, y el control de productos, órdenes y categorías. Todo esto construido con tecnologías modernas como Laravel 11 y React 18, utilizando buenas prácticas de desarrollo.

## Sección de mesas  
Proyecto enfocado en la gestión de un restaurante. Cuenta con un apartado para visualizar todas las mesas junto a las secciones en las que se divide el local, permitiendo un mayor orden. Estas mesas pueden encontrarse en diferentes estados, ya sea disponibles, ocupadas o en proceso de pago, lo que dependerá directamente de si existe una orden asociada a dicha mesa. La persona que atiende al cliente tiene la posibilidad de buscar productos por su nombre o identificador si así lo desea. Además, se pueden agregar notas personalizadas para ciertos productos, en caso de que el cliente requiera características específicas (como sal, condimentos, tipo de cocción, entre otros).

Si el cliente lo solicita, también se puede cambiar de mesa durante el servicio. Al momento de abrir una mesa, es posible registrar observaciones relacionadas con peticiones del cliente o cualquier característica que el trabajador que atiende haya notado.

## Sección de cocina y bar  
En este apartado se visualizan todas las comandas activas que contienen productos pendientes por preparar. Si un producto es cocinado y marcado como entregado, desaparecerá automáticamente del listado. Si es el último producto en la comanda, entonces será la comanda completa la que dejará de mostrarse en pantalla.

Dado que la dinámica puede variar según el funcionamiento interno de cada restaurante, se aplicó esta forma flexible de gestionar los productos solicitados a cocina o bar. En algún momento se consideró implementar un sistema de anclado de comandas (pin) para priorizar ciertos pedidos, dejando el resto en espera hasta que un cocinero pueda atenderlos. Sin embargo, esto dependerá de múltiples factores como la cantidad de estaciones en cocina, el número de cocineros, o si se trabaja directamente con una pantalla o con comandas impresas, entre otros aspectos.

## Sección de administración  
Desde aquí se gestionan los productos, categorías y mesas. Principalmente, se desarrollaron módulos CRUD para dar soporte a los distintos procesos del sistema que dependen de estos recursos.

Existe también un apartado de órdenes, donde se puede visualizar un listado con todas las órdenes actuales en curso, así como aquellas que ya fueron procesadas. Se puede acceder al historial completo de lo ocurrido, con la posibilidad de editar los detalles por parte del administrador (esta funcionalidad puede cambiar con el tiempo).

## Futuras implementaciones

- Separación de vistas por rol  
- Implementación de autenticación  
- Sección de perfil  
  - Mis ventas  
  - Mi cuenta  
  - Cerrar sesión  
- Mantenedor de usuarios  
- Sección de movimientos (ingresos, egresos)  
- Sección de reportes (gráficos)  
- Sección de arqueo de caja  

## Dependencias del proyecto  
La cantidad de dependencias puede ser mayor en el lado del front-end.

- Laravel 11  
- Laravel Sanctum (Auth API)  
- Tailwind v3  
- React v18  
- React Query  
- React Router  
- Zustand
