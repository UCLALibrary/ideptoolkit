---
layout: page
title: Transferencia de MiniDV
menu: true
order: 6
lang: Español
ref: minidv
permalink: /minidv-spa
---

### Lista de equipos:

1. Máquina reproductora de video digital Sony modelo HVR-M25AU (y cable r AC)
![](../assets/img/minidv/video_deck.png)

2. Cable FireWire 800/400 de 9 pines a 6 pines
![](../assets/img/minidv/firewire.png)

3. Adaptador Apple de Thunderbolt a FireWire. **Para reparaciones de cinta necesarias (4-6):**
![](../assets/img/minidv/firewire_adapter.png)

4. Cinta de empalme de ¼ pulgada
![](../assets/img/minidv/splicing_tape.png)

5. Destornillador Phillips de 1.4mm
![](../assets/img/minidv/screwdriver.png)

6. Hoja de afeitar de borde único o tijeras afiladas.
![](../assets/img/minidv/razor.png)
<br>**Para limpiar los cabezales de video cuando se obstruyen (7-8):**

7. Hisopos libres de pelusa (para limpiar los cabezales de video)
![](../assets/img/minidv/swabs.png)

8. Alcohol Isopropílico (99%) (para limpiar los cabezales de video)
![](../assets/img/minidv/alcohol.png)

### Antecedentes del MiniDV

El MiniDV es un formato de video introducido en 1995. Su tamaño pequeño y calidad visual lo hicieron especialmente popular en el mercado del consumidor y en el educacional. Cada cinta puede almacenar alrededor de 13GB para grabar cerca de una hora de video. En promedio el tiempo de reproducción es de alrededor de 60 minutos si se graba en modo estándar (SP) o de 90 minutos en modo extendido (LP).

![](../assets/img/minidv/tape.png)

Como otros formatos de videocintas DV, la cinta magnética dentro del cassette MiniDV es de ¼ de pulgada de ancho, por lo que cualquier reparación puede realizarse con cinta de empalme de ¼ de pulgada, usada típicamente en trabajo con materiales de audio. Aunque las reparaciones físicas son requeridas con poca frecuencia, las técnicas de reparación se revisarán brevemente al final de este documento.

![](../assets/img/minidv/tape2.png)

Las cintas MiniDV pueden ser reproducidas en la mayoría de las máquinas DVCAM. El reproductor Sony que han recibido (Modelo HVR-M25AU) tiene un mecanismo de doble tamaño de cassette que acepta tanto tamaños mini como estándar de cintas de video DigitalMaster, DVCAM y DV. Nota: ciertas cintas MiniDV marca Panasonic no pueden ser reproducidas en máquinas reproductoras Sony.

La codificación almacenada en las cintas MiniDV puede ser Digital Video (DV), DVCAM o HDV. La señal de video de todos estos formatos es comprimida o &quot;con pérdida de información&quot;. Sin embargo, la señal de audio para DV es no-comprimida. La frecuencia de muestreo (número de muestras de audio por segundo) y la profundidad de bits (número de bits usados para transportar los datos en cada muestra de audio) pueden variar.

El DV funciona con los siguientes modos de audio lineal modulado por pulsos codificados (PCM):
* 4 canales a 12 bits con una frecuencia de muestreo de 32 kHz
* 2 canales a 16 bits con frecuencia de muestreo de 48 kHz
* 2 canales a 12 bits con modo 32 kHz
* 2 canales a 16 bits con frecuencia de muestreo de 44.1 kHz (similar a la frecuencia de muestreo de los CDs)

![](../assets/img/minidv/sampling_rate.png)

DVCAM es una versión semi-profesional del formato DV y puede ser reproducido a una velocidad mayor. El formato de video HDV está codificado con esquema de compresión H.262/MPEG-2 y su audio estéreo está codificado con el esquema de compresión MPEG-1 Layer 2. El audio y video comprimidos se unen en una pista de transporte MPEG-2. La relación de aspecto de las pistas de video de MiniDV pueden ser estándar (4:3) o de pantalla ancha (widescreen, 16:9):

![](../assets/img/minidv/ratio.png)

Para este proyecto capturaremos la pista de datos de video a través de una conexión FireWire que preservará los datos de la forma más exacta, incluyendo sus metadatos originales.  FireWire también se conoce como i.LINK. La transferencia de la pista a través de las salidas tradicionales de video como componente o S-video alteraría los datos.

![](../assets/img/minidv/s-video.png)

### Transfiriendo contenido de un MiniDV

El software que usarán para transferir contenido en DV y DVCAM se llama AVCVideoCap. Es una herramienta del Apple FireWire SDK versión 26, un kit de desarrollo de softwares para sistemas operativos Mac. AVCVideoCap es un excelente candidato para la preservación de MiniDV porque transmite las señales de datos en bruto (o raw) sin aplicar cambios ni a la imagen ni al sonido. El archivo master resultante en bruto puede ser codificado a una gran variedad de archivos derivados.

Sin embargo, AVCVideoCap no puede capturar contenido HDV. Para cintas que contengan HDV, usarán DVHSCap. Ambos flujos de trabajo serán explicados más abajo.

![](../assets/img/minidv/avcvideo.png)

**Conectar los cables y encendido:**
  1. Conecta el cable entregado en el conector AC IN en la parte trasera del reproductor Sony HVR-M25AU DV. Conecta el otro extremo a la fuente de energía.
  2. Conecta el cable FireWire 800/400 de 9 pines/6 pines a la entrada i.LINK en la parte trasera del reproductor DV. La conexión de 6 pines se conecta al reproductor DV.
  3. Conecta el extremo de 9 pines del FireWire al adaptador Apple FireWire a Thunderbolt.
  4. Conecta el adaptador Thunderbolt al MacBook Pro.
  5. Enciende la unidad DV antes de encender tu computadora.
      * Presiona el interruptor de encendido en la parte trasera de la unidad a &quot;ON&quot;.
      * Presiona el botón de encendido en la parte delantera del reproductor.

**Preparar la transferencia de MiniDV:**
1. Asegúrate que tu MiniDV se encuentre en &quot;Modo Seguro&quot; para que no sea posible grabar sobre el contenido accidentalmente.
![](../assets/img/minidv/mode.png)
2. Introduce tu cinta MiniDV. Suave, pero con firmeza empuja la cinta dentro de la compuerta.
3. Rebobina la cinta si no se encuentra aún al inicio de la grabación.
4. Presiona &quot;Play&quot; y revisa brevemente la relación de aspecto y las especificaciones de audio y video. La pantalla LCD ubicada en la parte delantera del reproductor mostrará la imagen. El sonido puede ser monitoreado con audífonos conectados a la salida verde en la parte delantera del reproductor. La frecuencia de muestreo de audio de la grabación se mostrará automáticamente en la pantalla LCD. Asegúrate que el Audio Mode (Modo de Audio) del reproductor está ajustado para igualar la frecuencia original de la grabación. Para hacer esto ve a: Menu&gt;Audio Set (Configuración de Audio)&gt;Audio Mode. Aquí puedes ajustar entre 48 kHz o 32 kHz.

**Iniciar la transferencia de DV/DVCAM:**
1. Para DV o DVCAM abre el software de captura llamado AVCVideoCap ya sea:
  * Tecleando AVCVideoCap en el campo de búsqueda de Spotlight en Mac, o
    * Yendo a: **Macintosh HD&gt;Developer&gt;FireWireSDK26&gt;Applications&gt;AVCVideoCap.app**

2. Selecciona la unidad DV en la lista de dispositivos
![](../assets/img/minidv/screenshot.png)
3. Haz clic en &quot;Capture from Device&quot; (Captura desde el dispositivo). Nombra el archivo y selecciona la ubicación en el disco duro donde será guardado. Luego haz clic en &quot;Save&quot; (Guardar).
![](../assets/img/minidv/screenshot_2.png)
4. A continuación, en modo de grabación, selecciona &quot;Tape Control&quot; (Control de Cinta), luego selecciona &quot;Continue&quot; (Continuar).
![](../assets/img/minidv/tape_control.png)
5. El MiniDV comenzará automáticamente a reproducir y transmitir datos DV o DVCAM. Cuando esté completo la cinta se detendrá automáticamente. Si deseas detener la captura en cualquier momento, selecciona &quot;Abort Capture Now&quot; (Abortar la Captura Ahora). El video digital resultante tendrá una extensión .DV.
![](../assets/img/minidv/screenshot3.png)

**Iniciar la transferencia de contenido HDV:**
1. Para HDV abre el software de captura llamado CVHSCap ya sea:
  * Tecleando DVHSCap en el campo de búsqueda de Spotlight en Mac, o
  * Yendo a **Macintosh HD&gt;Developer&gt;FireWireSDK26&gt;Applications&gt;DVHSCap.app**

2. Elige &quot;Capture from D\_VHS&quot; (Captura desde D-VHS).
![](../assets/img/minidv/screenshot4.png)
3. Nombra tu proyecto y selecciona &quot;Save&quot; (Guardar) en la ventana &quot;Select Capture File&quot; (Selecciona Archivo de Captura). Selecciona la ubicación en tu disco duro para capturar el video.
![](../assets/img/minidv/screenshot5.png)
4. El MiniDV comenzará automáticamente a reproducirse y a transmitir datos HDV. Cuando esté completo la cinta se detendrá automáticamente. Si deseas detener la captura en cualquier punto, selecciona &quot;Stop Capture&quot; (Detener Captura). El video digital resultante tendrá una extensión .m2t.
![](../assets/img/minidv/screenshot6.png)

### Crear archivos streaming para acceso

Además de los archivos en bruto (raw) .dv y .m2t que guardarás para preservación, crearás archivos mp4 más livianos para acceso en streaming

1. Inicia Adobe Media Encoder
  * Teclea Adobe Media Encoder en el campo de búsqueda de Spotlight de Mac o,
  * Ve a: Launchpad &gt; Adobe Media Encoder
2. Arrastra al Queue (fila) los archivos .dv y .m2t que quieres transcodificar.
![](../assets/img/minidv/access1.png)
3. Selecciona cada ítem en la fila y en &quot;Format&quot; (Formato) selecciona H.264 de la lista desplegable de estándares de video.
![](../assets/img/minidv/access2.png)
4. En &quot;Preset&quot; (Ajustes guardados), selecciona &quot;UCLA Library - Video - Streaming File&quot;. Las especificaciones de este ajuste son:
  * Pista de Video: H.264/mp4 -AVC, SD, 480p
  * Pista de Audio: 32kHz/16-bit AAC
![](../assets/img/minidv/access3.png)
5. En &quot;Output File&quot; (Archivo resultante) haz clic sobre el nombre del archivo para seleccionar una ubicación para guardar los archivos.
6. Repite los pasos 3-5.
7. Una vez que tienes una fila de archivos lista para ser transcodificada, haz clic en el ícono verde de reproducción para comenzar la codificación. Procesarás los archivos idealmente al final del día de trabajo para permitir que los procesos se ejecuten durante la noche.
![](../assets/img/minidv/access4.png)

### Reparar cinta MiniDv

Una cinta MiniDV podrá necesitar reparación ocasionalmente. La cinta puede haberse roto o el cassette original puede tener un problema que impide su reproducción. La cinta rota puede repararse con cinta de empalme de ¼ pulgada. Si la caja del cassette está dañada puede ser reemplazada por la de  una cinta MiniDV virgen.

![](../assets/img/minidv/New Picture.bmp)

1. La mayoría de las cintas MiniDV tienen cuatro tornillos pequeños ubicados en la parte inferior del cassette. Usando un destornillador de estrella pequeño (de tamaño aproximado 1.4mm), remueve los cuatro tornillos. Ten cuidado de no dejar que la cinta dentro del cassette se desenrolle o se dañe. Pon los tornillos en un lugar seguro de manera de que sean ubicados fácilmente cuando termines. Si la cinta no tiene tornillos tendrás que romper el cassette cuidadosamente para poder remover los rollos de forma segura.
![](../assets/img/minidv/tape_repairing.png)  ![](../assets/img/minidv/tape2_repairing.png)
2. Luego, junta las puntas cuidadosamente, asegurándolas con un pedazo pequeño de cinta de empalme por el lado brillante. No pongas cinta en la superficie mate u opaca pues este lado contiene la grabación. Corta cuidadosamente la cinta de empalme que sobra por los lados del borde de la cinta. Se recomienda utilizar guantes al manipular la cinta para evitar dañar la superficie grabada (a pesar del mal ejemplo de la foto de abajo).
![](../assets/img/minidv/tape3_repairing.png)
Para prevenir que la cinta se desenrolle mientras trabajas, puedes asegurarla con un trozo de cinta.
![](../assets/img/minidv/tape4_repairing.png)
3. Si el cuerpo del cassette está dañado, puedes traspasar los rollos a una nueva caja de cassette previamente desensamblada. Remueve cuidadosamente los rollos del cassette viejo y ponlos en la nueva carcasa. Elimina las partes de cinta floja rebobinando los rollos manualmente.
![](../assets/img/minidv/tape5_repairing.png)
4. Una vez que la reparación esté completa, ubica en su posición la cubierta y para asegurar cierra el cassette atornillando.
