# Proyecto de Servicios de Limpieza

Este proyecto es un sitio web que ofrece servicios de limpieza. Utiliza Sass para una mejor organización del código CSS y emplea un diseño modular.

### Variables de Color
- **`$text-color`**: Color del texto principal del sitio.
- **`$bg-primary`**: Color de fondo para el botón primario.
- **`$bg-primary-hover`**: Color de fondo cuando el botón primario es hover.
- **`$bg-secondary`**: Color de fondo para el botón secundario.
- **`$bg-secondary-hover`**: Color de fondo cuando el botón secundario es hover.
- **`$bg-card`**: Color de fondo para las tarjetas de servicio.

### Variables de Tipografía
- **`$font-family-base`**: Tipografía base utilizada en todo el sitio.
- **`$font-size-large`**: Tamaño de fuente para elementos grandes (títulos).
- **`$font-size-small`**: Tamaño de fuente para textos pequeños.

### Variables de Espaciado y Bordes
- **`$padding`**: Espaciado uniforme para los elementos.
- **`$border-radius`**: Radio de los bordes aplicados a botones y tarjetas.
- **`$transition-time`**: Tiempo de transición para las animaciones.

## Funciones utilizadas

### transition

- La propiedad transition permite crear efectos de transición suaves entre diferentes estados de un elemento. Se utiliza en botones y tarjetas para mejorar la experiencia del usuario al interactuar con ellos.

```scss
.btn {
    transition: all 0.2s ease-in;
}

.card {
    transition: all 0.2s ease-in;
}
```

### transform

- La propiedad transform permite aplicar transformaciones 2D y 3D a los elementos. En este proyecto, se utiliza para crear un efecto de "elevación" al pasar el mouse sobre las tarjetas.

```scss
.card:hover {
    transform: translate(0, -30px);
}
```

### flex

- El modelo de caja flexible (flexbox) es utilizado para crear layouts más eficientes y responsivos. Se usa para alinear y distribuir el espacio entre los elementos en contenedores flexibles.

```scss
.section-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    align-items: center;
    gap: 20px;
}
```

### box-shadow

- La propiedad box-shadow añade sombras alrededor de un elemento, lo que proporciona profundidad y mejora la apariencia visual. Se usa en las tarjetas para darles un efecto de elevación.

```scss
.card {
    box-shadow: 10px 10px 0 rgb(27, 27, 27);
}
```