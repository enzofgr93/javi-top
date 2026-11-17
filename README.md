# Javi Top

Run and gun estilo Contra, ambientado en un MediaMarkt. Javi recorre los pasillos
de Samsung, Xiaomi, Vivo, Motorola y Pixel, y acaba en la zona de cajas contra Estherina.
Hecho en HTML5 (canvas) y empaquetado como APK con Capacitor. Sin imágenes ni
archivos de audio: todo se dibuja y suena por código, así que el APK pesa muy poco.

## Niveles y jefes (8)

1. Vivo: jefe Manu (fácil)
2. Honor: Capitán Honor (media-fácil)
3. Motorola: jefa Marey (media)
4. OPPO: jefe Dani (media)
5. Xiaomi: jefe Ricardo (media-difícil)
6. Samsung: jefe Pau (media-difícil)
7. Apple: Maestro Apple (difícil)
8. MediaMarkt: jefa final Estherina, 3 fases (difícil)

Cada nivel tiene 4 zonas de emboscada con checkpoint, robots pesados y jefe final.

## Estilo

Todo transcurre dentro de una tienda MediaMarkt: pared de televisores, pasillos con productos, carteles de secciones, neveras, lavadoras, carros y palés. Sprites con contorno y sombreado tipo dibujo animado, explosiones animadas, casquillos, humo de misiles y brillo. Todo se genera por código.

## Extras

Protectores de pantalla enemigos (19.99€ y 24.99€). Al quedarte con 1 corazón sale un personaje a gritarte.

## Armas

S spread · L láser perforante · F lanzallamas · M misiles teledirigidos · G balas que rebotan.
Coger la misma arma otra vez la mejora (hasta 3 estrellas). R = disparo rápido, E = escudo, + = vida.

## Controles

- Móvil: flechas, ▲ apuntar arriba, SALTAR y FUEGO (en horizontal).
- Teclado: flechas o WASD, X/espacio saltar, Z disparar, P pausa.

## Cómo obtener el APK

1. Crea un repositorio nuevo en GitHub y sube todo el contenido de esta carpeta
   (incluida la carpeta oculta `.github`).
2. Ve a la pestaña **Actions**. El workflow "Build APK" se ejecuta solo al hacer push
   (también puedes lanzarlo con **Run workflow**).
3. Cuando termine (3-6 minutos), abre la ejecución y descarga el artefacto
   **javi-top-apk** (un .zip con `app-debug.apk`).
4. Descomprime, pasa el APK al móvil e instálalo (hay que permitir
   "instalar apps de orígenes desconocidos").

## Probar en el navegador

Abre `www/index.html` directamente.

Nota: es un APK de depuración (debug), válido para instalar y jugar,
pero no para publicar en Google Play.


## Novedades
- **Agacharse**: botón ▼ (o flecha abajo / S). Agachado se dispara y se es más difícil de alcanzar.
- **TOP**: sub-arma con barra de carga (se llena con el tiempo y con cada baja). Botón TOP (o tecla V). Lanza un enorme mensaje "TOP" que atraviesa enemigos, borra balas y hace mucho daño. Los cafés AICHA solo curan.
- **Icono**: carpeta `icon/` (JAVI TOP); el workflow lo copia al APK automáticamente.
- **Estilo arcade pixel-art**: el mundo se dibuja a 480x270, con paleta limitada, tramado ordenado y escalado sin suavizar. Botones de movimiento (◀ ▼ ▶ ▲) del mismo tamaño.
- **Audio**: sonido distinto por arma (pistola, spread, láser, llamas, misiles, rebote, TOP), explosiones con ruido y graves, pasos y aterrizaje. Música con batería, bajo, melodía y arpegio; cambia por nivel, y suena otra más rápida e intensa con los jefes.
- **Movimiento**: voltereta al saltar, salto con margen para pulsar un poco antes/después del borde, y apuntar hacia abajo en el aire (▼ + disparo).
- **2.5D (v12)**: motor 3D propio en WebGL (sin librerías externas). Escenario MediaMarkt con perspectiva real y profundidad (estanterías, columnas, techo con luces, pared de TVs, carteles), y personajes, enemigos y jefes modelados en 3D. La jugabilidad sigue siendo de avance lateral. Si el móvil no soporta WebGL, el juego usa automáticamente el modo 2D anterior.
