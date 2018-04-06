---
layout: page
title: Términos Descriptivos
menu: true
order: 3
lang: Español
ref: terms
permalink: /terms-spa
---
<!-- TOC depthFrom:1 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. Título (obligatorio)](#1-ttulo-obligatorio)
- [2. Nombre de Archivo &amp; Identificadores](#2-nombre-de-archivo-amp-identificadores)
- [3. Creador / Colaborador](#3-creador-colaborador)
- [4. Lugar de Publicación (Recomendado)](#4-lugar-de-publicacin-recomendado)
- [5. Fecha (Obligatorio)](#5-fecha-obligatorio)
- [6.  Idioma (Obligatorio)](#6-idioma-obligatorio)
- [7. Tipo (Obligatorio)](#7-tipo-obligatorio)
- [8. Descripción Física](#8-descripcin-fsica)
- [9. Institución/Repositorio (Obligatorio)](#9-institucinrepositorio-obligatorio)
- [10. Derechos (Obligatorio)](#10-derechos-obligatorio)
- [11. Descripción (Recomendado)](#11-descripcin-recomendado)
- [12. Tema (Recomendado)](#12-tema-recomendado)
- [13. Relación (Recomendado)](#13-relacin-recomendado)
- [14. Origen (Recomendado)](#14-origen-recomendado)

<!-- /TOC -->

### 1. Título (obligatorio)

##### DEFINICIÓN:

Una palabra, frase, caracter o grupo de caracteres que nombra el recurso que está siendo descrito.

##### GUÍA para crear valores para el elemento TÍTULO

Los títulos pueden ser **transcritos** o **asignados.** Un título transcrito aparece en el ítem. Si no hay un título inscrito en el ítem, es posible construir un título con los metadatos entregados por los participantes, entregados por el creador o la institución que posee el material, o tomado de un trabajo de referencia u otra fuente confiable. No es necesario poner paréntesis cuadrados para indicar que el título asignado no fue tomado a partir de la ítem.

No incluya artículos definidos o indefinidos al inicio del título. Use mayúsculas al estilo estándar americano.

```
Ejemplos
* Déjeuner sur l&#39;Herbe [ejemplo de título asignado]
* Papeles de la familia Bacot [asignado]
* Sonatas para violín y piano [transcrito]
* Pinturas australianas aborígenes sobre el SIDA [asignado]
* Paisajes citadinos de Los Ángeles en 1965 mirando al Noroeste hacia las montañas de Santa Mónica [asignado]
```

### 2. Nombre de Archivo &amp; Identificadores

##### Nombre de Archivo (obligatorio)

El nombre de archivo del objeto (ej. `arce_0001.tiff`) se guarda en el campo "**Filename**" (Nombre de Archivo). Para observar las mejores prácticas de nombres de archivos, ver la ["Guía de Nombres de Archivo &amp; Organización."](https://uclalibrary.github.io/ideptoolkit/filenaming.html)

##### Identificador

Un **Identificador** es un identificador universal tales como ISBN, ISSN, DOI, o un número OCLC.

##### ID Local (Recomendado)

Un **ID Local** es un identificador asignado de forma local. Este puede ser una marca de estante, número de ítem o número de catálogo, o en algunos casos el nombre de archivo sin la extensión (ej. `arce_0001`).

### 3. Creador / Colaborador

El elemento **CREADOR** es **obligatorio** (si es conocido), y el elemento COLABORADOR es recomendado.

##### DEFINICIÓN:

CREADOR: La entidad o entidades principales responsables de crear el contenido del recurso (i.e. autor, fotógrafo, artista, etc). Este elemento es obligatorio si el creador del recurso es conocido.

CONTRIBUIDOR: Aquellos responsables de hacer contribuciones al contenido intelectual o artístico, o la producción física y diseminación del recurso (i.e., editorial, traductor, editor, distribuidor, etc.)

##### GUÍA para la creación de valores para los elementos CREADOR y COLABORADOR

Es preferible tomar el nombre del creador y colaborador de un archivo estándar de nombres de autoridades. Para las colecciones IDEP, la autoridad preferida es el [Virtual International Authority File](https://viaf.org/) (Archivo Virtual de Autoridades Internacionales, VIAF). Si el nombre no se encuentra en VIAF, es posible usar otros archivos de autoridades como Library of Congress Name Authority File (LCNAF), Union List of Artists&#39; Names (ULAN), u otra autoridad nacional. Si un nombre no aparece en un archivo de autoridad, se puede ingresar en la hoja de metadatos usando la forma `APELLIDO, PrimerNOMBRE`.

En la columna **Autoridad,** indicar el código de la autoridad de la que se tomó el nombre (VIAF, LCNAF, ULAN, etc.). Si el nombre no aparece en un archivo de autoridades, el código de la fuente debe ser &quot; **local.&quot;**

En el caso de creadores múltiples y/o colaboradores (del mismo tipo), ingresa cada nombre separado por `/` en la celda. Para múltiples tipos de colaboradores (1 editor, 1 traductor), ingresa los nombres en columnas de COLABORADOR separadas. Las columnas de colaboradores deben ser clasificadas para indicar el rol (i.e. editorial, editor, etc.). Hay varias opciones disponibles en el menú desplegable. Si éstas no reflejan en forma precisa el rol, puedes consultar el [MARC Code List: Relator codes](https://www.loc.gov/marc/relators/relaterm.html) (Lista de Códigos de MARC: Códigos Relacionales) o el [ULAN role table](http://www.getty.edu/vow/ULANRolePopup) (Tabla de Roles ULAN).

Si el CREADOR es desconocido, aconsejamos que los colaboradores de metadatos usen el elemento **COLABORADOR.**

```
Ejemplos (Creador)
* Master de Saint Francis (Italiano, activo 2nd mitad del siglo 13) [ejemplo de un nombre de artista de ULAN]
* Diseño Big Deal (Compañía) [nombre del diseñador de LCNAF]
* Artista tahitiana desconocida [nombre de artista de un archivo de autoridad local (creado de acuerdo a la guía CCO)
```

```
Ejemplos (Contribuidor)
* Landsforeningen for bøsser og lesbiske [editorial, de LCNAF]
* Dickinson, John [diseñador, de ULAN]
```

##### Estándares y Guías
* [Virtual International Authority File](https://viaf.org) Archivo Virtual de Autoridades Internacionales (VIAF) - **Preferido**
* [Library of Congress Name Authority File](http://authorities.loc.gov) Archivo de Nombres de Autoridades de la Biblioteca del Congreso (LCNAF)
* [Union List of Artists&#39; Names](http://www.getty.edu/research/tools/vocabularies/ulan/) Lista Unificada de Nombres de Artistas (ULAN)

### 4. Lugar de Publicación (Recomendado)

##### DEFINICIÓN:

El nombre del lugar donde ha sido publicado un recurso. (El nombre del editor se guarda en el elemento **Colaborador.** )

##### GUÍA para la creación de valores para el elemento LUGAR DE PUBLICACIÓN

La forma del nombre del lugar debe ser tomada del objeto. Cuando el objeto no indique un lugar, utilice un archivo estándar de nombres de autoridades, tales como El Tesauro de Nombres Geográficos (TGN) o el Archivo de Nombres de Autoridades de la Biblioteca del Congreso (LCNAF).

```
EJEMPLOS
* Copenhagen (Dinamarca)
* Habana
```

##### Estándares y Guías

* [Tesauro de Nombres Geográficos (TGN)](http://www.w3.org/TR/NOTE-datetime)
* [Archivo de Nombres de Autoridades de la Biblioteca del Congreso (LCNAF)](http://authorities.loc.gov)

### 5. Fecha (Obligatorio)

##### DEFINICIÓN:

Un punto o período de tiempo asociado a un evento en el ciclo de vida del recurso (ej. creación, publicación, impresión, restauración, etc.).

##### GUÍA para la creación de valores para el elemento FECHA

La información de fecha puede ser tomada del mismo ítem, o de cualquier fuente confiable, tales como documentación relacionada al ítem, etc. Cuando las fechas exactas son desconocidas, los contribuyentes de metadatos deben proveer un rango de fechas posibles para el recurso, tales como la década o siglo en el cual fue creado o publicado. Utilizar el elemento Descripción para manifestar incertidumbres si es necesario.

Cuando hay múltiples tipos de fechas asociadas a un recurso y no es práctico guardarlas todas, la prioridad debe ser el tipo(s) que sea más importante para los usuarios. Por ejemplo, la fecha en que fue construido un edificio es probablemente más importante que la fecha en la que fue fotografiado o la fecha en la que la foto fue digitalizada.

Los contribuyentes de metadatos deben proveer fechas a un nivel apropiado de especificidad para el recurso. Si se conoce una fecha exacta relacionada al recurso, ésta debe ser proporcionada.

##### Las fechas deben ser entregadas en dos formatos:

* **Fecha de visualización:** adecuada para ser mostrada, ej. Agosto 26, 2016
* **Fecha normalizada:** permite el procesamiento automatizado (ej. filtros de búsqueda, ordenamiento de resultados). La fecha normalizada debe seguir el formato AAAA-MM-DD for ejemplo, 2016-08-26.

| Ejemplos | Fecha de Visualización | Fecha Normalizada |
| --- | --- | --- |
| Año de publicación | 1965 | 1965 |
| Rango de años posibles | Entre 1967 y 1985 | 1967/1985 |
| Lapso de fecha | 1993-1995 | 1993/1995 |
| Fecha exacta | Octubre 26, 1969 | 1969-10-26 |
| Siglo | Siglo 19 | 1801/1900 |
| Fecha estimada | Julio o Agosto 1991 | 1991-07/1991-08 |

##### Estándares y Guías

* [W3C: Formatos de fecha y hora](https://www.w3.org/TR/NOTE-datetime)

### 6.  Idioma (Obligatorio)

##### DEFINICIÓN:

Designación del idioma en el cual se expresa el contenido del recurso, o que es primordial para la comprensión del recurso. (Nota: No el idioma de la ficha de metadatos.)

##### GUÍA para la creación de valores para el elemento IDIOMA

Utilice el código ISO 639-3 para el idioma del recurso (ver abajo).

Si es un recurso no-textual, utilice el código **&#39;zxx&#39;** (contenido no lingüístico). Si no se puede determinar el idioma, utilice el código **&#39;und&#39;** (no se puede determinar un idioma).

```
EJEMPLOS
* ara [Árabe]
* eng [Inglés]
* jpn [Japonés]
```

Otros Estándares y Guías

* [Códigos para la representación de nombres de idiomas (ISO 639-3)](https://www.loc.gov/standards/iso639-2/php/code_list.php)

### 7. Tipo (Obligatorio)

##### DEFINICIÓN:

La naturaleza o género del contenido del recurso. Para describir el formato de archivo, medio físico, o dimensiones del ítem, utilice el elemento Descripción Física.

##### GUÍA para la creación de valores para el elemento TIPO

*Incluya siempre un clasificador para este elemento.*

Clasificadores requeridos:

**Type.collection (Tipo.colección)** – Elija uno de estos dos valores:

* sí - el récord es para una colección de recursos
* no – el récord es para un recurso individual

**Type.manuscript (Tipo.manuscrito)** – Elija uno de estos dos valores:

* sí – El recurso descrito es un manuscrito
* no - el recurso descrito no es un manuscrito

**Type.typeOfResource (Tipo.tipoDeRecurso)** – El tipo general de contenido del recurso. La plantilla de metadatos contiene un menú desplegable de términos aceptados (texto, imagen fija, cartografía, grabación sonora, imagen en movimiento, etc.)

**Type.genre (Tipo.género)** – Una categoría que caracteriza un estilo en particular, forma o contenido, tales como artístico, composición musical literaria, etc. Este clasificador permite más especificidad que los términos utilizados en el Type.typeOfResource. Utilice un vocabulario controlado (preferentemente el Art &amp; Architecture Thesaurus Online [Tesauro de Arte &amp; Arquitectura Online, AAT]) cuando sea posible; de lo contrario identifique el término como un encabezado local.

```
EJEMPLOS
* Type.collection: yes Type.manuscript: yes [Record para una colección de manuscritos digitalizados.]
* Type.collection: yes Type.manuscript: no [Record para una colección de posters digitalizados.]
* Type.collection: no Type.manuscript: yes [Record para un documento digital individual (por si mismo o como parte de una colección más grande).]
* Type.collection: no Type.manuscript: no [Record para un póster digital individual (por si mismo o como parte de una colección más grande).]
* Type.typeOfResource: imagen fija.
* Type.typeOfResource: grabación sonora.
* Type.genre: posters
* Type.genre: Periódicos.
* Type.genre: Spaghetti Westerns
```

**Otros Estándares y Guías**

Para **Type.genre** :

* **Tesauro de Arte &amp; Arquitectura Online (AAT)**  (preferido)
* Términos de Género Básicos para Materiales Culturales Patrimoniales (BGTCHM)
* Encabezados Temáticos de la Biblioteca del Congreso (LCSH)
* Vocabularios Controlados para la Sección de Libros Únicos y Manuscritos (RBMS)
* Tesauro para Materiales Gráficos (TGM)

### 8. Descripción Física

##### DEFINICIÓN:

El medio físico, largo o dimensiones del recurso. Este elemento es conocido en algunos esquemas de metadatos como &quot;formato&quot;.

##### GUÍA para la creación de valores para el elemento DESCRIPCIÓN FÍSICA

El elemento Descripción Física puede ser usado para registrar información sobre el recurso: largo, dimensiones y medio.

**PhysicalDescription.extent (DescripciónFísica.largo)** (Obligatorio) – Número de ítems, número de páginas o duración (largo por ejemplo en segundos) del recurso. (Puede ser el mismo tanto al referirse al recurso original como al objeto digital.)

**PhysicalDescription.dimensions (DescripciónFísica.dimensiones)** (Recomendado) – Las medidas del recurso original, incluyendo su tamaño o escala.

**PhysicalDescription.medium (DescripciónFísica.medio)** (Recomendado) – El material o soporte físico del recurso (i.e. los materiales de los que está compuesto el recurso).

```
EJEMPLOS
* PhysicalDescription.extent: 1 postal
* PhysicalDescription.dimensions: 61 x 43 cm. (24 x 17 in.) [poster]
* PhysicalDescription.extent: 95 min. [película]
* PhysicalDescription.dimensions: 161.5 cm. (circunferencia, esfera) [globo]
* PhysicalDescription.medium: marcador y tinta sobre papel.
```

### 9. Institución/Repositorio (Obligatorio)

##### DEFINICIÓN:

El nombre del repositorio donde el recurso está ubicado actualmente.

##### GUÍA para la creación de valores para el elemento INSTITUCIÓN/REPOSITORIO

Prefiera tomar el nombre de un archivo estándar de nombres de autoridad, tales como el Archivo de Nombres de Autoridades de la Biblioteca del Congreso (LCNAF). Si el nombre no aparece en el archivo de autoridades, establezcalo de acuerdo a un estándar de contenido tales como las Reglas Anglo-Americanas de Catalogación (AACR2), Catalogación de Objetos Culturales (CCO), o Describiendo Archivos: Un Estándar de Contenidos (DACS).

```
EJEMPLOS
* Charles E. Young Research Library. Departamento de Colecciones Especiales.
* Vorderasiatisches Museum (Berlin, Alemania)
```

### 10. Derechos (Obligatorio)

##### DEFINICIÓN:

Información sobre la creación y/o publicación de un recurso que está relacionado a los derechos de propiedad intelectual asociados al objeto.

##### GUÍA para la creación de valores para el elemento DERECHOS

*Siempre incluye clasificadores para este elemento.*

**Calificadores requeridos:**

**copyrightStatus (estadoDeDerechos):** sólo utiliza valores controlados.

* derechos activos – el material tiene derechos vigentes.
* dominio público - el material está en el dominio público (siguen valores más específicos de dominio público).
* dominio público – gobierno federal de EE.UU.
* dominio público – dedicado (significa que el beneficiario de los derechos ha reconocido el ítem como dominio público).
* dominio público – caduco (para algo cuyo derecho ha expirado).
* desconocido – si el estado de los derechos del ítem no se conocen.

**publicationStatus (estadoDePublicación):** Elige uno de los tres valores:

* publicado
* no publicado
* desconocido

**servicesContact (contactoDeServicios):** información de contacto de cualquier servicio ofrecido que esté relacionado a este ítem. Puede ser la información de contacto para solicitudes de derechos y/o solicitudes de imágenes master. Se recomienda proveer datos para este clasificador (especialmente a nivel de colección) para incentivar y permitir a los usuarios contactar a la unidad correcta para permisos, licencias y archivos de alta calidad.

```
EJEMPLOS
* Rights.copyrightStatus: activo
* Rights.publicationStatus: publicado
* Rights.servicesContact: Doe, John (jdoe@email.edu)
```

### 11. Descripción (Recomendado)

##### DEFINICIÓN:

Un registro del contenido del recurso y cualquier otra información descriptiva sobre el recurso. Descripción puede incluir información tal como un resumen, tabla de contenidos o un registro de texto libre sobre el contenido.

##### GUÍA para la creación de valores para el elemento DESCRIPCIÓN

Utiliza clasificadores para distinguir los distintos tipos de Descripción (por ej. resumen, inscripción, nota, etc.). Sé juicioso en el uso de este elemento; información importante sobre el recurso debe ser capturada en otros elementos si es apropiado.

```
EJEMPLOS
* Description.note: Fecha en parte posterior del poster, 1997, refleja la fecha en que fue recibido por el vendedor y luego cuando fue adquirida por la Biblioteca de UCLA.
* Description.inscription: Estudiantes de &quot;Longhaired&quot; Palisades High School protestan contra la demanda de la escuela que los obliga a cortarse el cabello.[tomada de una muestra del recurso.]
```

### 12. Tema (Recomendado)

Cualquiera de los tópicos o temas de una obra, indicados explícitamente en el recurso o su título o implícitamente en su contenido. Los temas pueden ser personas u organizaciones, otros recursos, lugares, o tópicos.

##### A. Personas / organizaciones

##### DEFINICIÓN:

Nombres significativos (personales, corporativos, familia, reunión) que son el sujeto del recurso, están representados en el recuerdo o por el recurso.

##### GUÍA para la creación de valores para el elemento TEMA

Prefiera tomar el nombre de un archivo estándar de nombres de autoridades como VIAF u otros como el Archivo de Nombres de Autoridades de la Biblioteca del Congreso (LCNAF) o la Lista Unificada de Nombres de Artistas (ULAN). Si el nombre no aparece en el archivo de autoridades, establezcalo de acuerdo a un estándar de contenido tales como las Reglas Anglo-Americanas de Catalogación (AACR2), Catalogación de Objetos Culturales (CCO), o Describiendo Archivos: Un Estándar de Contenidos (DACS).

```
EJEMPLOS
* Antoniani, Pietro, d ca. 1740-1805
* Instituto sin Fronteras.
```

##### B. Títulos

##### DEFINICIÓN:

Títulos significativos de otros recursos (por ej. obras, expresiones de esas obras, ítems individuales, etc.) que son el sujeto del recurso, están representados en en el recurso, o por el recurso.

##### GUÍA para la creación de valores para el elemento TEMA

La estructura del título debe ser extraída de un archivo estándar de nombres de autoridades como el Archivo de Nombres de Autoridades de la Biblioteca del Congreso, el que contiene títulos uniformes (LCNAF). Si el título no aparece en el archivo de autoridades, establezcalo de acuerdo a un estándar de contenido tales AACR2, CCO o DACS.

```
EJEMPLOS
* Biblia. O.T. Salmos
* Maha bha rata
```

##### C. Lugar

##### DEFINICIÓN:

Nombres significativos de locaciones geográficas que son el sujeto de o que están representados en el recurso o por el recurso.

##### GUÍA para la creación de valores para el elemento TEMA

La estructura del nombre de un lugar debe ser tomado de un archivo estándar de nombres de autoridades. Para IDEP recomendamos el Tesauro de Nombres Geográficos (TGN). Si el nombre no aparece en un archivo de autoridades, establezcalo de acuerdo a un estándar de contenido tales AACR2 o CCO.

IDEP utiliza formas jerárquicas para nombres de lugares, utilizando columnas separadas para:
* **Subject.country (Tema.país)**
* **Subject.city (Tema.ciudad)**
* **Subject.place (Tema.lugar)** ( para ubicaciones específicas dentro de una ciudad, región o país)

```
EJEMPLOS
* Subject.place: Acequia Madre de Santa Barbara
* Subject.country: Irán
* Subject.city: Yerevan
```

##### D. Tópico

##### DEFINICIÓN:

Una descripción o interpretación de los tópicos, actividades, eventos, ideas u objetos que son el sujeto del recurso, o que están representados en el recurso, o por el recurso. En el caso de imágenes, utiliza el elemento Tema para guardar tanto la temática del recurso (concepto) como también de qué se trata (descriptivo) si es que aplica.

##### GUÍA para la creación de valores para el elemento TEMA

La estructura del término Tema debe ser tomada de un tesauro estándar de temas, como LCSH, MeSH, AAT o TGM.

```
EJEMPLOS
* Etiquetas de cajas de fruta
* Depresión (Estado mental)
* Planificación Regional.
* antimacasas
```

### 13. Relación (Recomendado)

##### DEFINICIÓN:

Una referencia a un recurso relacionado. (Nota: para objetos que son parte de colecciones digitales, la Relación -- entre el objeto y la colección de la que forma parte -- se crea automáticamente.)

##### GUÍA para la creación de valores para el elemento RELACIÓN

*Este elemento debe ser siempre clasificado.*

La mejor recomendación es hacer referencia al recurso a través de un código o número que se ajuste a un sistema de identificación formal, siempre que sea posible.

Las relaciones pueden ser expresadas de forma recíproca (si los recursos son descritos en ambos extremos de la relación) o en sólo una dirección, incluso cuando hay un refinamiento disponible para permitir la reciprocidad. Si se usa texto simple en vez de un código formal o números de identificación, la referencia debe ser apropiadamente específica. Por ejemplo, se puede usar una cita bibliográfica formal para referir a los usuarios a un recurso en particular.

```EJEMPLOS
* Relation.hasVersion (Relacion.tieneVersion): Reporte IFDC (Edición en Español) [ejemplo de una versión en otra edición, idioma, etc.]
* Relation.hasFormat (Relacion.tieneFormato): Versión en CD-ROM: Alfabetismo de Salud. Washington, D.C. : National Academies Press, c2004.
* Relation.derivedFrom (Relacion.derivadoDe): Michelangelo Buonarroti, 1475-1564. Creación de Adán. [ejemplo de una obra inspirada en esta pintura]
```

### 14. Origen (Recomendado)

##### DEFINICIÓN:

Un recurso relacionado a partir del cual se genera el recurso descrito, por completo o en parte. Este elemento puede incluir también información sobre la historia de propiedad o de custodia del objeto.

##### GUÍA para la creación de valores para el elemento ORIGEN

La recomendación y mejor práctica es identificar el recurso relacionado a través de un código que se ajuste a un sistema de identificación formal, siempre que sea posible. En general, debe incluir en esta área información sobre un recurso que está relacionado intelectualmente al recurso que está siendo descrito, pero que no se ajusta fácilmente al elemento Relación.

Información sobre ubicación de un descubrimiento o excavación del objeto deben ser ingresada en el elemento **Tema** o el elemento **Cobertura.Espacial**  de la ficha.

Origen no será normalmente utilizado para objetos nativos digitales.

```
EJEMPLOS
* BM XV cent., II, p. 346 (IB.5874)
* Record del Archivo Smithsonian Unidad 54, Colección Joseph Henry, 1808, 1825-1878, Caja 1, Carpeta 6, Item 3.
```
