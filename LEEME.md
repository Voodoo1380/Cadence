--- LEEME para Cadence ---

Cadence es un set de herramientas usadas para la produccion de audio.
Esta siendo desarrollado por falkTX, usando Python3 y Qt5 (y algunos C++ cuando es necesario).

Las herramientas comparten el mismo codigo fuente base, asi que la mayoria se ven bastante parecidas (lon que es intencional).
Ademas, muchos de los custom widgets son codificados cuando es necesario (como pixmapdial, pixmapkeyboard, patchcanvas y systray).
Pueden ser re-usados en otros proyectos. Contacte al autor si necesita ayuda con esto.

===== DESCRIPCIONES =====

Aqui una breve descripcion de las herramientas principales:

Cadence

La aplicacion principal. Realiza comprobaciones del sistema, gestiona JACK, llama a otras herramientas y hace retoques del sistema.

Cadence-JackMeter

Medidor digital de picos para JACK.
Conecta automaticamente todas las aplicaciones a los puertos de salida de JACK que tambien estan conectados a la salida del sistema.

Cadence-JackSettings

Dialogo de configuracion simple y facil de usar para jackdbus.
Puede configurar el driver JACK y los parametros del motor, tambien soporta LADISH studios.

Cadence-Logs

Pequeña herramienta que muestra los logs de JACK, A2J, LASH y LADISH en una ventana multi-pestañas.
Los logs son visualizados en un cuadro de texto, haciendo facil navegar y extraer mensajes de estado usando los comandos copiar y pegar.

Cadence-Render

Herramienta para grabar (o 'renderizar') un projecto de JACK usando jack-capture, controlado por JACK Transport.
Soporta un vasto numero de tipos de archivo y puede renderizar en ambos modos, realtime y freewheel.

Cadence-XY Controller

Simple XY widget que envia y recibe datos desde Jack MIDI.
Puede enviar datos a traves de canales especificos y tambien es un teclado MIDI.

Catarina

Una aplicacion de testeo de Patchbay, creada mientras el modulo patchcanvas estaba siendo desarrollado.
Permite al usuario experimentar con el patchbay, sin usar ALSA, JACK o LADISH.
Puedes guardar y cargar configuraciones del patchbay tambien.

Catia

JACK Patchbay, con algunas caracteristicas cuidadas como soporte A2J bridge y JACK Transport.
It's supposed to be as simple as possible (there's Claudia for advanced things), so it can work nicely on Windows and Mac too.
Currently has ALSA-MIDI support in experimental stage (it doesn't automatically refresh the canvas when changes happen externally).

Claudia

LADISH frontend; como Catia, pero enfocada a la administracion de sesiones a traves de LADISH.
It has a bit more features than the official LADISH GUI, with a nice preview of the main canvas in the bottom-left.
It also implements the 'Claudia-Launcher' add-application style for LADISH.

Claudia-Launcher

Un lanzador de aplicaciones multimedia con soporte LADISH.
Busca paquetes instalados (no binarios), y muestra el contenido respectivo como un lanzador.
The content is got through an hardcoded database, created and/or modified to suit the target distribution.
Actualmente soporta distribuciones basadas en Debian y ArchLinux.
