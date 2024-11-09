# Sistema Solar en 3D

Este proyecto es una simulación de un sistema solar en 3D, donde se pueden visualizar diferentes cuerpos celestes, incluyendo el sol, planetas, lunas y asteroides. Cada cuerpo celeste tiene su propio shader que define su apariencia y comportamiento visual.

## Características

- **Cuerpos Celestes**: Incluye el sol, la Tierra, lunas, asteroides y un planeta de nubes.
- **Shaders Personalizados**: Cada cuerpo celeste tiene un shader único que simula texturas y efectos visuales.
  - **Shader del Sol**: Simula un efecto de lava dinámica.
  - **Shader de la Tierra**: Incluye un continente o isla verde.
  - **Shader de Nubes**: Simula nubes dinámicas y en movimiento.
  - **Shader de Asteroides**: Presenta texturas complejas con piscinas de lava.

## Controles

- **Teclas WASD**: Mover la cámara hacia adelante, atrás, izquierda y derecha.
- **Teclas de flecha (Arriba/Abajo)**: Rotar la cámara hacia arriba y hacia abajo.
- **Tecla Q**: Mover la cámara hacia arriba.
- **Tecla E**: Mover la cámara hacia abajo.
- **Tecla 1**: Acercar la cámara.
- **Tecla 2**: Alejar la cámara.
- **Tecla B**: Activar la vista de pájaro (bird's eye view), que posiciona la cámara directamente sobre el sistema solar, mirando hacia abajo.

## Requisitos

- Rust (versión 1.50 o superior)
- Cargo (gestor de paquetes de Rust)
- Dependencias de gráficos (como `nalgebra`, `rand`, etc.)

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/tu_usuario/sistema-solar-3d.git
   cd sistema-solar-3d
   ```

2. Instala las dependencias:

   ```bash
   cargo build
   ```

## Uso

Para ejecutar la simulación, utiliza el siguiente comando:

```bash
cargo run --release
```

## Estructura del Proyecto

- `src/`: Contiene el código fuente del proyecto.
  - `main.rs`: Archivo principal que inicializa la simulación y renderiza los cuerpos celestes.
  - `camera.rs`: Define la lógica de la cámara y su movimiento, permitiendo la navegación en el espacio 3D.
  - `color.rs`: Maneja la representación y manipulación de colores en la simulación.
  - `fragment.rs`: Contiene la lógica para los shaders de fragmento, que determinan el color de los píxeles.
  - `framebuffer.rs`: Administra el framebuffer para la renderización de la escena.
  - `obj.rs`: Define la carga y representación de modelos 3D en formato OBJ.
  - `planet.rs`: Define la estructura y comportamiento de los planetas en la simulación.
  - `shaders.rs`: Contiene los shaders para cada cuerpo celeste, definiendo sus texturas y efectos visuales.
  - `triangle.rs`: Maneja la lógica y representación de triángulos en la simulación.
  - `vertex.rs`: Contiene la definición de los vértices y su manipulación en la renderización.

