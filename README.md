# GFashion Guide

Guía HTML para principiantes de moda femenina (Argentina): nombres, siluetas y vocabulario para conversar sobre prendas.

## Cómo abrirla

1. Descargá `index.html` (y, si querés el ícono de pestaña, `favicon.svg`).
2. Abrilo con doble clic en el navegador de la computadora.

Por defecto arranca en **formato Computadora**. Arriba podés cambiar a **formato Teléfono** (marco de celular).

## Qué incluye

- Niveles: familia de prenda (Nivel 1) y variante (Nivel 2), con descripción concatenada.
- Filtro de temporada: Completa / Verano-Primavera / Invierno-Otoño. Lo atemporal y de media estación aparece en ambas.
- Ilustración flat por prenda y galería placeholder para fotos reales.

El contenido sigue [SPEC.md](SPEC.md).

## Comparación experimental con Fashion-MNIST

La interfaz muestra, junto a la ilustración original, una referencia visual de Fashion-MNIST cuando existe una correspondencia directa o una silueta razonablemente cercana. El dataset original de Zalando Research contiene 10 clases de imágenes en escala de grises de 28×28 px: T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag y Ankle boot.

La comparación es deliberadamente experimental: Fashion-MNIST no representa accesorios como sombreros, bufandas, collares, aros, cinturones o anteojos, ni muchas variantes específicas como stilettos o ballerinas. En esos casos la interfaz indica que no existe una correspondencia directa en lugar de forzar una equivalencia.

Las imágenes de referencia se cargan desde el sprite oficial del repositorio zalandoresearch/fashion-mnist y se mantiene la atribución correspondiente a su licencia MIT (Copyright © 2017 Zalando SE).
