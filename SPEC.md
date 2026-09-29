# SPECIFICATION DOCUMENT: Manual/Guía Básica de Moda Femenina

## 1. Resumen del Proyecto y Público Objetivo

Este documento define el contenido, la estructura de datos y las especificaciones de interfaz para un manual HTML sobre moda femenina, orientado al uso cotidiano en Argentina.

**Público Objetivo:** La guía está diseñada para principiantes absolutos. El objetivo es proporcionar las herramientas visuales y el vocabulario necesario para identificar prendas y sus variantes en la calle, permitiendo mantener una conversación básica con alguien conocedor. El lenguaje será descriptivo, directo y accesible.

## 2. Especificaciones de Interfaz (UI) y Experiencia (UX)

### 2.1. Layout, Disposición y Dinámica de Niveles

La interfaz mostrará el contenido utilizando una jerarquía interactiva de dos niveles: **Categoría General (Nivel 1)** y **Subcategoría/Variante (Nivel 2)**.

* **Ilustración principal:** Mostrará un diseño representativo de la Categoría General o cambiará dinámicamente si se selecciona una variante.
* **Seudo-galería (Placeholder):** Contenedor preparado para cargar fotos reales posteriormente.
* **Interacción Nivel 1 -> Nivel 2:**
  1. Al seleccionar una prenda de **Nivel 1** (ej. "Zapatos de Taco"), se mostrará su título y una descripción base de la familia de prendas.
  2. Debajo de esta descripción base, aparecerá una lista interactiva (botones o etiquetas) con las opciones de **Nivel 2** (ej. "Stilettos", "Taco Cuadrado").
  3. Al hacer clic en una opción de Nivel 2, la descripción se actualizará concatenando la información. La estructura visual será: *"Los \[Nivel 1\] se caracterizan por \[Descripción Base\]. Por su parte, los tipo \[Nivel 2\] se destacan dentro del grupo por \[Descripción de la Subcategoría\]"*.
* **Ubicación del texto:**
  * *Desktop:* A la **derecha** de la ilustración.
  * *Mobile:* **Debajo** de la ilustración.

### 2.2. Navegación y Filtros

* **Barra Superior (Top Bar):** Incluirá un menú desplegable (Dropdown).
* **Filtro de Temporada:** `Verano / Primavera`, `Invierno / Otoño`, o vista completa (`Atemporal` aparece en ambas).

### 2.3. Especificaciones de Assets Gráficos

* **Ilustraciones:** `.SVG` o `.PNG` (fondo transparente), relación 1:1 (300x300px o 400x400px). Buscar estilo "flat design" en Freepik, Flaticon o unDraw.
* **Galería de Imágenes (Futuro):** `.WEBP` o `.JPG`, miniaturas de 150x150px expandibles.

## 3. Estructura de Datos y Glosario de Prendas

### 3.1. Accesorios de Cabeza y Cuello

* **Gorros y Sombreros**
  * *Descripción Nivel 1:* Accesorios diseñados para usarse sobre la cabeza. Pueden tener una función térmica (como abrigar en invierno) o estética y protectora (como cubrirse del sol).
  * *Subcategorías (Nivel 2):* 
    * **Gorrito de lana (Beanie):** `[Invierno/Otoño]` Se destacan por ser tejidos, ajustados a la forma del cráneo, cubriendo las orejas y, en muchas ocasiones, llevando un doblez en el borde o un pompón arriba.
    * **Piluso (Bucket hat):** `[Atemporal]` Se destacan por tener forma de balde invertido, con un ala circular, corta e inclinada hacia abajo que da sombra a los ojos y la nuca.

* **Bufandas y Pañuelos**
  * *Descripción Nivel 1:* Prendas de tela o lana que se envuelven alrededor del cuello. Son el complemento de abrigo por excelencia en los meses fríos.
  * *Subcategorías (Nivel 2):*
    * **Bufanda manta (Maxibufanda):** `[Invierno/Otoño]` Se destacan por ser piezas de tela o tejido extremadamente grandes y anchas, al punto de que, desdobladas, pueden cubrir los hombros o el torso entero como un pequeño chal.

### 3.2. Joyería y Bisutería

* **Collares**
  * *Descripción Nivel 1:* Accesorios ornamentales que se llevan alrededor del cuello. Pueden ser discretos y sutiles o piezas grandes que toman el protagonismo del look.
  * *Subcategorías (Nivel 2):*
    * **Cadenita (Fina con dije):** `[Atemporal]` Se destacan por ser hilos de metal muy delgados y sutiles que caen sobre el pecho, generalmente acompañados de un pequeño adorno colgante (dije).
    * **Gargantilla (Choker):** `[Atemporal]` Se destacan por ir completamente ceñidas y ajustadas al cuello, sin colgar. Pueden ser de tela, cuero, terciopelo o eslabones de metal.

* **Aritos y Aretes**
  * *Descripción Nivel 1:* Accesorios que se llevan en las orejas. Tienen el poder de iluminar el rostro y pueden transformar un look básico en uno mucho más producido.
  * *Subcategorías (Nivel 2):*
    * **Argollas:** `[Atemporal]` Se destacan por su forma de anillo cerrado o semi-abierto que atraviesa el lóbulo. Pueden ser finitas y pequeñas, o muy grandes y gruesas (chunky).
    * **Abridores / Puntos de luz:** `[Atemporal]` Se destacan por ser diminutos y quedar pegados directamente sobre el lóbulo de la oreja, habitualmente formados por una pequeña perlita, bolita de metal o piedra brillante.
    * **Aros Colgantes:** `[Atemporal]` Se destacan por extenderse hacia abajo, superando el lóbulo de la oreja. Suelen tener movimiento y diseños más elaborados para eventos o salidas.

### 3.3. Ropa de Torso

* **Remeras y Tops**
  * *Descripción Nivel 1:* Prendas superiores ligeras y de uso casual que se llevan directamente sobre la piel, generalmente hechas de algodón o telas elásticas.
  * *Subcategorías (Nivel 2):*
    * **Remera Básica:** `[Atemporal]` Se destacan por su corte clásico (cuello redondo o en 'V', mangas cortas) y por no tener estampados. Son el lienzo en blanco o "comodín" de cualquier conjunto.
    * **Musculosa:** `[Verano/Primavera]` Se destacan por no tener mangas, dejando los hombros y los brazos completamente al descubierto. Suelen tener breteles finos o gruesos.
    * **Top / Crop top:** `[Verano/Primavera]` Se destacan por ser prendas cortadas transversalmente, diseñadas intencionalmente para dejar el abdomen, el ombligo o la cintura al descubierto.

* **Camisas y Blusas**
  * *Descripción Nivel 1:* Prendas superiores generalmente abotonadas en el frente, con cuello, hechas de telas menos elásticas. Aportan un aire más formal o arreglado al atuendo.
  * *Subcategorías (Nivel 2):*
    * **Camisa Oversize:** `[Atemporal]` Se destacan por tener un corte deliberadamente grande, ancho y largo (como si fuera un talle o dos más grande de lo necesario). Da un aspecto relajado y urbano, y suele usarse desprendida con un top abajo o atada a la cintura.

* **Sweaters y Tejidos**
  * *Descripción Nivel 1:* Prendas de punto, cerradas o con botones, diseñadas específicamente para aportar abrigo en el torso sin necesidad de ponerse una campera pesada.
  * *Subcategorías (Nivel 2):*
    * **Sweater / Pullover:** `[Invierno/Otoño]` Se destacan por ser tejidos cerrados (sin botones ni cierres) que deben pasarse obligatoriamente por la cabeza para ponérselos.
    * **Cárdigan:** `[Invierno/Otoño]` Se destacan por ser abrigos de punto que vienen abiertos en la parte delantera, cerrándose generalmente con una hilera de botones.

### 3.4. Abrigos

* **Camperas**
  * *Descripción Nivel 1:* Prendas de abrigo exteriores que suelen llegar hasta la cadera o cintura, con cierre o botones frontales. Varían muchísimo en grosor y estilo.
  * *Subcategorías (Nivel 2):*
    * **Campera Puffer:** `[Invierno/Otoño]` Se destacan por estar acolchadas y divididas en costuras horizontales o geométricas, dándoles un aspecto inflado (como un "plumífero"). Suelen ser de tela sintética y muy abrigadas.
    * **Campera Biker (Motoquera):** `[Atemporal / Media Estación]` Se destacan por ser generalmente de cuero o cuerina, cortas a la cintura, con cierres metálicos cruzados en el frente y solapas llamativas. Dan un look rebelde y urbano.

* **Tapados y Pilotos**
  * *Descripción Nivel 1:* Abrigos más largos que suelen sobrepasar la cadera o llegar hasta las rodillas. Dan una silueta más elegante y estructurada.
  * *Subcategorías (Nivel 2):*
    * **Trench / Piloto:** `[Atemporal / Media Estación]` Se destacan por ser abrigos ligeros, de largo hasta la rodilla, cruzados en el frente con botones y que suelen llevar un cinturón de la misma tela. El color clásico es el beige o caqui.
    * **Tapado de paño:** `[Invierno/Otoño]` Se destacan por estar confeccionados en lana o telas gruesas y pesadas, con cortes rectos o entallados, botones grandes y solapas. Son la opción elegante por excelencia para el frío.

### 3.5. Pantalones

* **Jeans (Denim)**
  * *Descripción Nivel 1:* Pantalones fabricados en tela de mezclilla (denim). Son rígidos o semi-elásticos, muy duraderos y el pilar fundamental del estilo urbano cotidiano en Argentina.
  * *Subcategorías (Nivel 2):*
    * **Jean Wide Leg:** `[Atemporal]` Se destacan por tener piernas muy anchas que caen rectas desde la cadera (o cintura alta) hasta el suelo, sin ajustarse en ningún punto. Son la tendencia más fuerte de la moda urbana reciente.
    * **Jean Mom:** `[Atemporal]` Se destacan por ser de tiro alto (llegan al ombligo o más arriba), más sueltos en la zona de las caderas y muslos, y afinarse ligeramente hacia los tobillos. Tienen un aire retro de los años 90.

* **Pantalones de Tela**
  * *Descripción Nivel 1:* Pantalones confeccionados en telas distintas al jean (como lino, gabardina o algodón liviano). Pueden verse muy formales (para la oficina) o totalmente informales.
  * *Subcategorías (Nivel 2):*
    * **Pantalón Sastrero:** `[Atemporal]` Se destacan por su corte formal tipo "traje", generalmente con pinzas en la cintura y caída recta. Hoy en día son clave en la calle, usados de forma informal con zapatillas.
    * **Pantalón Cargo:** `[Atemporal]` Se destacan por tener múltiples bolsillos grandes y cuadrados, cosidos con solapa en los laterales exteriores de las piernas. Dan un look utilitario muy relajado.

* **Pantalones Deportivos / Confort**
  * *Descripción Nivel 1:* Pantalones diseñados priorizando la máxima comodidad y elasticidad. Nacieron para el gimnasio pero hoy son clave en la calle.
  * *Subcategorías (Nivel 2):*
    * **Calza (Legging):** `[Atemporal]` Se destacan por ser pantalones completamente elásticos que van totalmente ceñidos y apretados a las piernas desde la cintura hasta los tobillos, calcando la forma del cuerpo.

### 3.6. Faldas y Vestidos

* **Faldas**
  * *Descripción Nivel 1:* Prendas de vestir que cuelgan de la cintura hacia abajo sin división para las piernas, variando drásticamente en su largo (desde la mitad del muslo hasta los tobillos).
  * *Subcategorías (Nivel 2):*
    * **Falda Midi:** `[Atemporal]` Se destacan por su longitud específica: terminan a mitad de la pantorrilla, entre la rodilla y el tobillo. Pueden ser ajustadas o sueltas, y dan un aire sofisticado.
    * **Minifalda (Tabla o Jean):** `[Verano/Primavera]` Se destacan por ser muy cortas, terminando a mitad del muslo. Las de tablas (estilo colegial) y las de jean rígido son las más populares.

* **Vestidos**
  * *Descripción Nivel 1:* Prenda de una sola pieza que cubre desde el torso hasta las piernas. Simplifican el armado de un conjunto al ofrecer un look completo de manera instantánea.
  * *Subcategorías (Nivel 2):*
    * **Vestido Lencero (Slip Dress):** `[Verano/Primavera]` Se destacan por estar hechos de telas sedosas, ligeras y con caída fluida, colgados de breteles muy finos (espagueti). Imitan la estética de la lencería elegante.
    * **Vestido Camisero:** `[Verano/Primavera]` Se destacan por estar diseñados como una camisa de botones tradicional (con cuello y mangas), pero lo suficientemente larga como para usarse como vestido. Suelen llevar un lazo en la cintura.

### 3.7. Zapatos

* **Zapatos de Taco** `[Temporada: Atemporal]`
  * *Descripción Nivel 1:* Calzado que eleva el talón respecto a la punta del pie, diseñado tradicionalmente para estilizar la pierna o para eventos formales.
  * *Subcategorías (Nivel 2):*
    * **Stilettos:** Se destacan por tener un taco aguja (muy fino y generalmente alto) y una punta estrecha. Son el clásico zapato de fiesta elegante.
    * **Taco Cuadrado (Bloque):** Se destacan por tener un taco grueso y recto, lo que los hace mucho más estables, cómodos y de uso más informal.
    * **Sandalias de plataforma:** `[Temporada: Verano]` Calzado abierto que suma altura, ya sea con una suela alta y pareja, o combinando un taco grueso con plataforma en la parte delantera.

* **Zapatillas (Sneakers)** `[Temporada: Atemporal]`
  * *Descripción Nivel 1:* Calzado originalmente deportivo o informal que hoy es la base del uso diario urbano por su comodidad.
  * *Subcategorías (Nivel 2):*
    * **Urbanas (Lonas):** Se destacan por ser chatas, ligeras y de materiales como lona o cuero fino (ej. Converse, Vans). No tienen estética de "gimnasio".
    * **Chunkys / Running:** Se destacan por tener suelas exageradamente grandes y gruesas, o diseños deportivos técnicos (con mallas respirables o burbujas de aire).

* **Botas** `[Temporada: Invierno/Otoño]`
  * *Descripción Nivel 1:* Calzado cerrado de media estación o invierno que cubre el pie y se extiende por encima del tobillo o hasta la rodilla.
  * *Subcategorías (Nivel 2):*
    * **Borcegos:** Se destacan por ser botas acordonadas de cuero grueso con suelas de goma pesadas (estilo militar o de trabajo). Muy populares para uso diario.
    * **Tejanas (Cowboy):** Se destacan por tener un corte en "V" en la parte superior, costuras decorativas, punta afilada y un taco levemente inclinado hacia adentro.
    * **Botinetas:** Se destacan por ser botas cortas que llegan justo al nivel del tobillo, muchas veces ajustadas y con un pequeño taco fino o cuadrado.

* **Zapatos Planos (Flats)** `[Temporada: Atemporal]`
  * *Descripción Nivel 1:* Calzado cerrado, formal o semi-formal, que no presenta elevación en el talón.
  * *Subcategorías (Nivel 2):*
    * **Mocasines:** Se destacan por ser zapatos cerrados sin cordones. Actualmente en Argentina es tendencia usarlos con suela gruesa (chunky) y medias blancas a la vista.
    * **Chatitas (Ballerinas):** Se destacan por ser ultra planas y tener un escote amplio y redondeado en la parte superior, dejando el empeine al descubierto.

### 3.8. Bolsos y Complementos

* **Carteras y Bolsos**
  * *Descripción Nivel 1:* Accesorios funcionales diseñados para transportar objetos personales. Su tamaño y forma cambian drásticamente el estilo general del atuendo.
  * *Subcategorías (Nivel 2):*
    * **Tote Bag:** `[Atemporal]` Se destacan por ser bolsos grandes, abiertos en la parte superior (muchas veces sin cierre), con dos manijas paralelas largas para colgar del hombro. Suelen ser de lona o ecocuero y son ideales para cargar muchas cosas en el día a día.
    * **Riñonera:** `[Atemporal]` Se destacan por ser bolsos pequeños unidos a un cinturón ajustable. Aunque originalmente iban en la cintura, la tendencia actual urbana es usarlas cruzadas sobre el pecho o la espalda.
    * **Bandolera:** `[Atemporal]` Se destacan por tener una correa larga diseñada específicamente para cruzarse sobre el torso, apoyando el bolso en la cadera contraria. Permiten tener las manos totalmente libres.

* **Complementos**
  * *Descripción Nivel 1:* Accesorios adicionales que suman un detalle de estilo y funcionalidad, sirviendo muchas veces para "cerrar" visualmente un look.
  * *Subcategorías (Nivel 2):*
    * **Anteojos Cat-Eye:** `[Atemporal]` Se destacan por tener marcos donde las puntas superiores exteriores son puntiagudas y se elevan hacia arriba, imitando el ojo rasgado de un gato. Tienen un aire retro muy marcado.
    * **Cinturón Western:** `[Atemporal]` Se destacan por tener hebillas metálicas grandes, llamativas y labradas, muchas veces acompañadas de una puntera de metal haciendo juego al final del cinto. Aportan una estética "vaquera" que levanta cualquier jean básico.
