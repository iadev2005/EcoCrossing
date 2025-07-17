# EcoCrossing

## Instalación y Ejecución

### Método 1: Ejecutar con Java IDE
1. Requisitos previos:
   - Java JDK 19 o superior
   - Apache Maven
   - Un IDE de Java (NetBeans, Eclipse, IntelliJ IDEA)

2. Pasos:
   - Clonar el repositorio
   - Abrir el proyecto en tu IDE
   - Ejecutar `mvn clean install` para instalar las dependencias
   - Ejecutar la clase principal `com.mycompany.ecocrossing.EcoCrossing`
   - También es posible ejecutar directamente desde el ID dándole Play

### Método 2: Ejecutar con archivo .desktop (Linux)
1. Requisitos:
   - Sistema operativo Linux
   - Permisos de ejecución

2. Pasos:
   - Copiar el archivo `EcoCrossing.desktop` a tu escritorio
   - Hacer doble clic en el archivo
   - El juego se instalará y ejecutará automáticamente
   - Si es la primera vez, se te pedirá permiso para instalar las dependencias necesarias

### Notas de Instalación
- El juego requiere conexión a internet para el modo multijugador
- Para jugar en red local, asegúrate de que todos los jugadores estén en la misma red
- El primer jugador debe iniciar como servidor
- Los demás jugadores deben conectarse usando la IP del servidor

[![Gameplay](https://img.youtube.com/vi/eK2xFxtNus8/0.jpg)](https://www.youtube.com/watch?v=eK2xFxtNus8)

## Características Técnicas

### Arquitectura
- Desarrollado en Java utilizando programación orientada a objetos
- Sistema multijugador en tiempo real usando sockets UDP
- Arquitectura Cliente-Servidor
- FPS constante a 60 cuadros por segundo

### Características del Juego
- Soporte para múltiples jugadores simultáneos
- Sistema de colisiones avanzado
- Gestión de eventos y estados del juego
- Sistema de diálogos interactivos
- Inventario y comercio entre jugadores
- Sistema de sonido con música y efectos
- Interfaz de usuario dinámica

### Networking
- Comunicación en tiempo real mediante UDP
- Sistema de paquetes para sincronización de:
  - Movimiento de jugadores
  - Estado de objetos
  - Interacciones
  - Comercio
- Manejo automático de conexiones/desconexiones
- IP dinámica para conexiones remotas

## Créditos

### Desarrolladores
1. Ignacio Aliendres
   - Github: [@iadev2005](https://github.com/iadev2005)

2. Carlos Méndez
   - Github: [@carlos19men](https://github.com/carlos19men)

3. María Sandoval
   - Github: [@wildeswt](https://github.com/wildeswt)

4. Samuel Guzmán
   - Github: [@notoriussss](https://github.com/notoriussss)

### Inspiración
Este proyecto fue inspirado por los siguientes tutoriales y recursos:
- [Tutorial de RyiSnow](https://www.youtube.com/watch?v=om59cwR7psI&list=PL_QPQmz5C6WUF-pOQDsbsKbaBZqXj4qSq)
- [Tutorial de Zigurous](https://www.youtube.com/watch?v=7mlLlRjFDK8&list=PLvPPkch7E3t3GtccgGhFgtRxp6dyIAWvx)

## Controles del Juego

### Movimiento
- **W** o **↑**: Moverse hacia arriba
- **S** o **↓**: Moverse hacia abajo
- **A** o **←**: Moverse hacia la izquierda
- **D** o **→**: Moverse hacia la derecha

### Acciones
- **R**: Interactuar con objetos
- **Q**: Hablar con NPCs
- **C**: Abrir menú de personaje/inventario
- **P**: Pausar/Reanudar juego
- **ESPACIO**: Cerrar diálogos
- **ENTER**: Confirmar selección

### Menús
- En los menús usa **W/S** (o **↑/↓**) para navegar entre opciones
- En el inventario usa **W/A/S/D** (o flechas) para moverte entre ranuras
- **ESC**: Volver al menú anterior (en algunos estados)

### Comercio/Intercambio
- Usa las flechas o **W/A/S/D** para navegar por los objetos
- **ENTER** para seleccionar/confirmar
- **ESC** para volver al menú anterior

### Notas
- El juego tiene diferentes estados (menú principal, jugando, pausa, diálogo, comercio, etc.)
- Los controles pueden variar ligeramente dependiendo del estado del juego
- Algunos estados especiales como el comercio tienen sus propios controles específicos
