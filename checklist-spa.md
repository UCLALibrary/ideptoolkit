---
layout: page
title: Lista de Verificación (Impresos/Imágenes)
menu: true
order: 5
lang: Español
ref: checklist
permalink: /checklist-spa
---

###  Ajustes de Cámara

Asegúrese de que:
* El foco esté ajustado a **A** en el lente
* ISO está ajustado a **100**
* MODE está ajustado a **M**
* La apertura está ajustada entre f8 y f11 (comienza con f8)
* La velocidad de obturador está ajustada entre 1/60vo y 1/125vo (60-125 en el visor) (comienza con 60)
* Balance de blancos (WB) está ajustado a 5000K
* Calidad de imagen (QUAL) está ajustada a RAW

###  Ajuste de Cámara
* Instale la cámara en el trípode
* Conecte el remoto de obturador a la cámara
* Conecte el remoto de flash TTL a la parte superior de la cámar
* Remueva la tapa del lente de la cámara.
* Conecte la cámara al computador portátil.
* Abra y ajuste Lightroom
	* Asegúrese de que Lightroom abre en el catálogo en el que está trabajando (ej. "posters\_soviéticos" o "posters\_de\_films")
	* Del menú de File (Archivo), elija Tethered Shooting (Captura Conectada), luego comience la captura.
	* Ajustes:
		* Dele un nombre a la sesión (ej. sovietico02, film03, etc.)
		* Junto a Template (Plantilla), seleccione Edit (editar) del menú desplegable.
			* En el cuadro de texto, borre el patrón que aparece ahí.
			* Ingrese el prefijo del nombre de archivo seguido de un guión bajo `_`(ej. `soviético_`)
			* En la sección Number (número), seleccione Sequence # (secuencia) (00001) e Insert (Insertar)
			* La plantilla debe ser algo como: `sovietico_Secuencia # (00001)`
			* Haga click en Done (Listo)
			* Haga click en OK.

###  Ajusta el Pack de Batería Light &amp; el Remoto de Flash TTL

En Pack de Batería:
* Revise para asegurarte de que las luces están conectadas al pack de batería.
* Encienda el pack de batería
* Ajuste el canal del pack de batería a 1
* Presione SYNC hasta que esté ajustado a AIR
* Ajuste los niveles de luz a 8 (comience con 8, luego vaya subiendo o bajando para ajustar si es necesario)

En el Remoto de Flash TTL:
* Encienda el Remoto de Flash TTL (ON)
* Ajuste el canal a 1 (o el mismo canal ajustado en el pack de batería)
* Ajuste MODE a MAN

### Tomar fotografías
* Primero tome una fotografía con el Passport ColorChecker
* Comience capturando cada poster
	* Monte el poster
	* Capture la fotografía
	* Guarde el localID (número en la parte trasera del poster) en el campo "Copy Name" (copiar nombre) en la sección de Metadatos.
	* Repita hasta que todos los posters estén fotografiados.

### Finaliza la Captura

* Ponga la tapa en el lente de la cámara
* Remueva la cámara del trípode
* Revise las baterías de la cámara y el Remoto de Flash TTL - ¿necesitan ser cargados?
* Apague la cámara &amp; Remoto de Flash TTL
* Remueva y cargue (cámara) o reemplaza (Remoto de Flash TTL) las baterías si se necesita.
* Apague el pack de batería light
* Presione el botón blanco del pack de batería light para descargar la potencia remanente.
* Desconecte los cables del pack de batería light.
* Remueva la batería del pack de batería light y cárgala.

### Post-procesamiento (en Lightroom)

En la pestaña Develop (desarrollo), corte y alinee las imágenes.

Crear un Perfil de Color Checker por sesión
* Exportar la imagen con Color Checker al Escritorio como DNG
	* Selecciona la imagen
	* Del menú File (Archivo), seleccionar Export (Exportar)
	* Settings (Ajustes):
		* Exportar a: Desktop (Escritorio)
		* Formato de imagen: DNG
	* Haga click en el botón Export (Exportar) (esto guardará la imagen de referencia en su escritorio)
* Abra el software Color Checker Passport
* Tome y arrastre la imagen en la ventana de Color Checker
	* Espere que se cargue el perfil
	* Haga click en el botón "Create Profile" (Crear Perfil)
	* Nombre el nuevo perfil con el nombre de la sesión (ej. sovietico001)
* Cierre Color Checker Passport
* Cierre y reabra Lightroom para cargar el nuevo perfil.

Aplicar el perfil de ColorChecker a todas las imágenes de la sesión
* Abra Lightroom, selecciona la pestaña Develop (Desarrollo)
* Seleccione todas las imágenes de la sesión
* En la sección de Camera Calibration (Calibración de Cámara), selecciones el Perfil que acabas de crear desde el menú desplegable para aplicar a todas las imágenes seleccionadas (ej. sovietico001)

Exporte las imágenes en lotes como TIFF
* Seleccione todas las imágenes en la sesión actual
* Del menú File (Archivo), elige Export (Exportar)
* Ajustes:
	* En Export Location (Ubicación de Exportación), elija el destino para exportar archivos (Escritorio o un disco duro externo), marque "Put in a Subfolder" (Poner en una subcarpeta), y asigne un nombre a la carpeta nueva
	* En File Naming (Nombre de Archivo), seleccione "Rename To:" (Renombrar a:) y selecciones Edit (Editar) del menú desplegable
	* En la ventana Filename Template Editor (Editor de Plantillas de Nombre), añadir "Filename_Copy Name" (NombredeArchivo_Copiar Nombre) en el editor de plantillas usando los botones Insertar (ver imagen abajo), luego seleccione Done (Listo)
	* En la sección File Settings (Ajustes de Archivo), asigne la extensión de archivo a TIFF
	* Exporte

Entregue el disco externo con el nuevo lote de imágenes al equipo de metadatos. ¡Listo!
