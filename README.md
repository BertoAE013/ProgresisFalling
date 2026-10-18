# Game Design Document: Babarcante

## 1. Visión General del Proyecto

* **Título Provisional:** Babarcante ()babosa & Mercante)

* **Género:** Plataformas 3D en primera persona / Gestión de tiempo y tienda.

* **Perspectiva:** Primera persona (FPP).

* **Motor Recomendado:** Unity

## 2. Concepto Principal y Lore

El jugador encarna a **Blingbombarguer**, un pequeño Slime gelatinoso que administra la tienda de suministros y antigüedades más famosa del reino subterráneo.

Los clientes acuden al mostrador de la tienda a pedir objetos específicos. Sin embargo, la tienda no tiene estanterías comunes: detrás del mostrador se encuentra el **Gran Almacén**, un enorme complejo vertical lleno de trampas, plataformas, zonas viscosas y atajos que conecta con distintos biomas y niveles.

## 3. Mecánicas Principales de Juego (Core Gameplay Loop)

```
[Cliente solicita pedido] ➔ [Inicio de Temporizador] ➔ [Recorrido de Plataformas en el Almacén] 
        ➔ [Recoger Objeto] ➔ [Regreso rápido al Mostrador] ➔ [Entrega + Recompensa]

```

### 3.1. Habilidades del Slime (Movimiento en 1ª Persona)

Al ser un Slime, la movilidad es el factor clave para superar las secciones de plataformas:

* **Salto Elástico (Charge Jump):** Mantener presionado el botón de salto para comprimirse y salir disparado hacia arriba o adelante.

* **Adherencia (Wall-Slide/Sticky Surface):** Posibilidad de pegarse temporalmente a paredes de piedra o madera para rebotar o escalar.

* **Desplazamiento Viscoso (Dash/Slide):** Deslizarse a gran velocidad por pendientes o suelos resbaladizos.

* **Dividirse/Encogerse (Unlockable):** Habilidad avanzada para pasar por tuberías o grietas estrechas sacrificando temporalmente masa.

### 3.2. Gestión de Pedidos y Tiempo

1. **Atención al Cliente:** Cada cliente llega al mostrador con una orden (ejemplo: *"Necesito 1 Cristal de Fuego y 2 Engranajes de Cobre"*).

2. **Tiempo Límite:** Cada pedido activa una barra de paciencia del cliente. Si el tiempo expira, el cliente se marcha enfadado y se pierde reputación.

3. **Multi-pedidos:** A medida que avanza el día, múltiples clientes pueden esperar simultáneamente en la tienda, requiriendo planificar la mejor ruta en el almacén para recoger varios objetos en un solo viaje.

## 4. Diseño del Almacén y Niveles

El almacén no es un simple cuarto, es un hub gigante conectado a varias áreas interconectadas:

* **Zona Central (El Almacén Principal):** Estanterías gigantes, cintas transportadoras, poleas y cajas apiladas. Diseñado para verticalidad.

* **Bioma 1: Las Tuberías Anegadas:** Zona con corrientes de agua que empujan al jugador, plataformas flotantes y válvulas.

* **Bioma 2: Las Calderas Rúnicas:** Zonas de lava o calor donde el Slime debe alejarse de los puntos de calor 

* **Bioma 3: El Archivo Cristalino:** Plataformas frágiles de cristal que se rompen al saltar sobre ellas y espejos de teletransporte.

## 5. Progreso y Recompensas

* **Monedas de Oro:** Obtenidas al completar entregas a tiempo (con bonos por rapidez).

* **Mejoras de la Tienda:**

  * Comprar tubos neumático

  * Extender la paciencia de los clientes mediante mejoras en la sala de espera.

* **Mejoras del Slime:**

  * Mayor fuerza de salto.

  * Mayor capacidad para cargar objetos múltiples sin perder velocidad.

## 6. Interfaz de Usuario (UI) y Arte

* **Estilo Artístico:** *Intencion “Cartoon”*

* **Visión en 1ª Persona:**

  * Efectos visuales en los bordes de la pantalla (gotas de gelatina al saltar o chocar fuerte).

* **UI In-Game:**

  * Un reloj de arena o temporizador visual.

  * Un holograma/icono flotante en la esquina que muestra los objetos solicitados en el pedido activo.
