# Para Plober

Gracias por adquirir una `TronXY X3A MKS` - Impresora FDM, de estilo CoreXY
Dimensiones maximas (supuestamente): `220x220x300` (nota: en la config siempre usé 200x200x200 de safe-zone)

NOTA: en `folder_content_desc` encontrarás info de que es cada folder

## Post-its
Esto es lo primero que hacia al enchufarla:

`Control > Motion > Z-offset = 0.58`

Despúes en otro post-it tengo anotado:
- Llevar todo a `0°C`
- LLevar el nozzle a `235°C`
- Limpiarlo
- Empezar desde `0.56` hasta `0.58` (ndt: asumo que se refiere al valor del otro post-it)
- Llevar nozzle a `242°C` y cama a `50°C`
- Volver a imprimir



_A continuación una lista de tips y software que usé_



# Software para la impresora 3D

## (1) Repetier (gratis, anda en linux!)
Version utilizada por mi: 2.2.2 (según copyright notice ~2019)
URL: https://www.repetier.com/

**Sirve para poder realmente generar el codigo para llevar a la impresora 3D**

Necesitas usar "CuraEngine" puesto de slicer (el software que convierte modelo en gcode) 
y configurarlo creando un perfil nuevo. Te adjunto screenshots y algunos archivitos 
de configuracion (de windows)

Tenes que configurar el espacio de trabajo, temperatura, nozzle, filamentos
(Con este software generas el G-Code que despues podes leer tipo txt)


## (2) MeshMixer (gratis para win-64bits o mac-universal -vas a tener que usar wine-)
Version utilizada por mi: 3.5.474 (según copyright notice ~2017)
NOTA: Si lo usas en win Desactivale el data collection!
URL: https://meshmixer.org/

Nota: arribe a este software despues de MUCHO renegar buscando un lugar donde tuviese muchas tools juntas.
Es super quirky, raringo, se re nota que autodesk se lo compro a otra gente, porque es todo no-intuitivo,
pero lamentablemente ES SUPER UTIL y aveces hasta necesario.

**Usado principalmente para convertir modelos en STL o fixearlos, cosas como:**
- Agregar SOPORTES!!! <- muy importante
- Rellenarlos (para que sean "solidos") y/o cerrar caras, huecos, o cosas que no corresponden en modelos reales <- muy importante
- Cortar con planos/corregir posición para la cama de impresión
- Borrar vertices lineas o caras sueltas
- Low-poly-zar
- Partir con operaciones booleanas modelos grandes en "pedazos" imprimibles
- Mergear, fusionar, modificar tamaños, rotacion, posicion etc (aca es donde te decia que el eje es otro)


## (3) OpenScad (gratis, anda en linux!)
Nose que verison tengo pero es ~2021
URL: https://openscad.org/
nota: parece que re va en linux (ver https://openscad.org/downloads.html)

**La mejor forma de describirlo es: "Codigo a 3D"**

Features
- Codigo a 3D. Por ejemplo un cubo se define asi `cube([10, 10, 10]);`
- Parametrizable. Por ejemplo pones `width = 50;` al comienzo del archivo, si despues cambias width todo se ajusta automagicamente.
- Integración directa con Thingiverse. Los archivos `.scad` (si estan bien escritos) directamente se visualizan 3D en la pagina `https://www.thingiverse.com/`.


# Random stuff

- *Hexagonal Flower Pot (twisted) for Succulents*
https://www.thingiverse.com/thing:2841595

(mas cosas: https://www.thingiverse.com/sebastian_p/makes)

- *El soporte para laptop que me preguntaste*
https://www.thingiverse.com/thing:1278085

- *El coso para "lijar" minis*
https://www.thingiverse.com/thing:2404850

- *Random chess set*
https://www.thingiverse.com/thing:7224734