# Levantamientos · cómo publicarla e instalarla en el iPad

La app funciona sin internet. Solo necesitas conexión **dos veces**:

1. En el computador, para publicarla en GitHub. Lo haces una sola vez.
2. En el iPad, para instalarla. También una sola vez.

Después abre y funciona siempre sin señal.

---

## Paso 1. Crear la cuenta de GitHub (en el computador)

1. Entra a **github.com** y toca **Sign up**.
2. Escribe tu correo, una contraseña y un **nombre de usuario**.
   - El usuario queda en el enlace de la app. Por ejemplo, con el usuario `andrescorrea` el enlace será `andrescorrea.github.io/levantamientos`.
   - Usa solo letras minúsculas, números o guiones.
3. Confirma el código que GitHub te manda al correo.
4. Si te pregunta por un plan, elige el **gratuito (Free)**.

## Paso 2. Crear el repositorio

1. Arriba a la derecha toca **+** y luego **New repository**.
2. En **Repository name** escribe: `levantamientos`
3. Déjalo en **Public**. El plan gratuito solo publica páginas de repositorios públicos.
   - Lo público es el programa, no tus levantamientos. Tus proyectos se guardan solo en el iPad y nunca se suben a GitHub.
4. Toca **Create repository**.

## Paso 3. Subir los archivos

1. Descomprime el .zip que te entregué en el computador.
2. En la página del repositorio que acabas de crear, toca el enlace **uploading an existing file**.
3. Arrastra **todos los archivos sueltos** de la carpeta. No arrastres la carpeta, sino lo que hay dentro:
   - `index.html`
   - `sw.js`
   - `manifest.json`
   - `three.min.js`
   - `jspdf.umd.min.js`
   - `icon-180.png`, `icon-192.png` e `icon-512.png`
   - `INSTRUCCIONES.md` (opcional)
4. Espera a que suban todos y toca **Commit changes**.

## Paso 4. Activar la página

1. En el repositorio, entra a **Settings** y, en el menú de la izquierda, a **Pages**.
2. En **Source** elige **Deploy from a branch**.
3. En **Branch** elige **main** y la carpeta **/ (root)**. Toca **Save**.
4. Espera 1 o 2 minutos y recarga. Arriba aparecerá el enlace de tu app, por ejemplo `https://andrescorrea.github.io/levantamientos/`.
5. Ábrelo en el computador para comprobar que carga.

## Paso 5. Instalarla en el iPad (con internet una sola vez)

Si el iPad no tiene Wi-Fi, compártele los datos del iPhone:

- **En el iPhone:** Ajustes → Punto de acceso personal → activa **Permitir a otros conectarse**.
- **En el iPad:** Ajustes → Wi-Fi → elige el nombre de tu iPhone.

Con el iPad conectado:

1. Abre **Safari** y escribe el enlace de tu app.
2. Cuando cargue, toca el botón **Compartir** (el cuadro con la flecha hacia arriba).
3. Toca **Agregar a pantalla de inicio** y luego **Agregar**.
4. Abre la app **desde el ícono nuevo** y espera unos 10 segundos con internet todavía activo. En ese momento la app se guarda completa en el iPad.
5. Desconecta el internet o pon el iPad en modo avión, cierra la app y ábrela de nuevo desde el ícono. Si abre, ya quedó lista para trabajar sin conexión.

---

## Trabajar con el Apple Pencil

- **El lápiz dibuja y arrastra. El dedo mueve el plano**, y con dos dedos se hace zoom. Si no tienes el lápiz a mano, activa **Dedo** en la barra.
- **Muro:** toca el punto de inicio y arrastra. El muro se ajusta a 90° y a las esquinas, y la medida aparece mientras dibujas. Sigue desde el punto naranja; cuando termines en el punto inicial, el espacio se cierra solo.
- **Cara de medición (como la línea de referencia de ArchiCAD):** al tocar **Muro** aparece el cuadro flotante **Muro nuevo**. Ahí eliges con los dibujos si tus medidas son por la **cara interior**, el **eje** o la **cara exterior**, el espesor y el redondeo del largo.
  - Lo que dibujas o escribes se mide sobre esa cara (la línea naranja del dibujo) y el espesor crece hacia el otro lado. El área del espacio siempre se calcula por dentro.
  - En un espacio ya hecho se cambia en **Datos → Medidas tomadas por**.
  - Las distancias de puertas y ventanas se miden desde la esquina de esa misma cara.
- **Todo se redondea:** lo que dibujas o arrastras con el lápiz sale de 10 en 10 cm. Eso vale para los muros, las losas, las cubiertas, los cortes, las escaleras, el tamaño de los elementos, la posición y el ancho de puertas y ventanas, las alturas en los alzados y al correr un muro o una esquina.
  - En el cuadro de cualquier herramienta puedes cambiar el redondeo a 5 cm o a 1 cm. Queda igual para todas las herramientas.
  - Si llegas a una esquina existente, se pega exacto a esa esquina.
  - Lo que **escribes** en el cuadro de medidas o en una cota se respeta tal cual (por ejemplo 3.12).
- **Medida exacta:** toca la cota de un muro, escribe la medida y toca OK.
  - Antes, elige **Fija inicio** o **Fija final**: esa esquina se queda quieta (cuadrito naranja) y el muro crece hacia la otra. Todo lo que está más allá de la esquina libre se corre con ella, como estirar en ArchiCAD.
- **Puerta, Ventana y Vano:** toca el muro donde va y arrástralo a su sitio. Los puntos de los extremos cambian el ancho.
- **Cubierta:** al tocar la herramienta eliges la forma y la dibujas con el lápiz.
  - **Rectangular, bóveda o anillo/estadio:** arrastra de una esquina a la otra.
  - **Forma libre:** toca cada esquina y toca la primera para cerrar.
  - **Polígono regular** (eliges el número de lados), **circular (cono) o cúpula:** arrastra del centro hacia afuera.
  - Si solo tocas dentro de un espacio, la cubierta toma su forma (también en L, T o U) con un alero de 0.50 m.
  - **Cada lado es un agua o un hastial**, con su propia pendiente. Las cumbreras, limatesas y limahoyas se calculan solas.
  - **Para estirar una agua,** arrastra el punto naranja del medio de ese lado: el alero se corre y la cubierta se recalcula.
  - Si tocas ese punto sin arrastrar, eliges el lado y arriba puedes ponerlo en agua o hastial, cambiar su pendiente, dividirlo o quitarlo.
  - Los puntos blancos de las esquinas cambian la forma. El círculo de arriba gira la cubierta.
  - En **Datos** pones la altura del alero, la pendiente de cada lado, el material y el estado. En la cúpula y la bóveda pones la flecha (altura); en el anillo, el ancho y hacia dónde cae el agua.
  - El PDF y el DXF traen una hoja de **planta de cubiertas**, y el cuadro muestra el área en planta y el área inclinada.
- **Espacios:** el nombre y el área solo aparecen cuando el espacio queda cerrado. Mientras esté abierto, se ve como "Muros abiertos".
  - Para volverlo espacio sin cerrarlo, tócalo y luego **Convertir en espacio**.
  - Toca los muros que lo forman; puedes sumar muros de otros tramos y quitar los que no van. El lado que falte se cierra con una línea punteada.
  - Toca **Listo** y escribe el nombre.
  - Después puedes cambiarle el nombre o los muros.
- **Mobiliario por familias:** en **Elemento** eliges la familia (Estructura, Instalaciones, Cocina, Baño, Zona de ropas, Sala, Comedor, Alcoba, Oficina, Exterior y vehículos) y luego el objeto.
  - Las camas, sofás, clósets y aparatos se pegan solos al muro, con el respaldo contra la pared.
  - En el DXF van en la capa MOBILIARIO.
- **Elemento** (columnas, vigas, aparatos, tanques…): elige el elemento, tócalo en el plano y arrástralo a donde quieras. Cerca de una esquina o de un muro se pega solo.
  - El círculo de arriba lo gira.
  - El punto de la esquina cambia su tamaño.
- **Tipos de puertas y ventanas:** al tocar Puerta o Ventana se abre la biblioteca. Elige el tipo y toca el muro donde va.
  - Puertas: batiente de 1 o 2 hojas, vaivén, corrediza, corrediza empotrada, plegable, pivotante, puerta-ventana, enrollable, garaje seccional y reja.
  - Ventanas: corrediza, batiente, proyectante, basculante, fija, guillotina, celosía y ventanal.
  - Para cambiar el tipo de una que ya pusiste, tócala y toca su nombre en la barra de arriba.
- **Pisos:** en el selector de abajo eliges el piso o tocas **+ Agregar piso**.
  - En **Datos** (sin nada seleccionado) defines el nombre, la cota y la altura de cada piso.
  - Al dibujar un piso de arriba, los muros del piso de abajo se ven de fondo como referencia.
- **Losa:** arrastra de esquina a esquina, o toca dentro de un espacio para crear la losa con su forma.
  - Arriba cambias el espesor y el nivel, o agregas un **vacío** (para escaleras o patios) tocando sus esquinas.
- **Escalera:** en el cuadro de la herramienta eliges el tipo (recta, en L, en U o caracol) y la huella, contrahuella y ancho que prefieres. Luego arrastras el lápiz desde el arranque **hasta donde llega**.
  - **La distancia que arrastras es el largo de la escalera.** Los escalones se reparten solos con la huella más cercana a la que escogiste. Por ejemplo, 1.50 m dan 5 escalones de 0.30. Mientras arrastras ves la escalera en naranja con el largo, los escalones y cuánto sube.
  - Ya dibujada, el **punto naranja del final** la alarga o la acorta con el lápiz. El **círculo** la gira libremente y el botón de girar la gira 90°.
  - En su cuadro escribes **Largo** (se reparte en los mismos escalones), **Escalones** (la contrahuella se queda igual y cambia lo que sube), **Contrahuella**, **Huella** y **Ancho**. Abajo te dice cuánto sube y si cumple la regla de Blondel.
  - Si solo tocas sin arrastrar, sale la escalera completa para la altura del piso.
- **Corte:** dibuja la línea de corte con el lápiz; la flecha indica hacia dónde se mira.
  - **Ver corte** lo abre en la pestaña **Cortes**, donde también están las 4 fachadas automáticas. Lo cortado sale relleno y lo de fondo en proyección, con los niveles de cada piso.
  - **Invertir vista** cambia el lado; **Profundidad** define hasta dónde se ve.
  - Los cortes y fachadas salen también en el PDF y en el DXF.
- **Fotos con medidas** (cocinas, baños, cuartos, fachadas…):
  - Con la herramienta **Foto** (la cámara de la barra) tocas en el plano el sitio donde estás y eliges **Tomar foto** o **Desde Fotos**. La foto queda marcada en el plano con una cámara (F1, F2…) y ligada a ese espacio. Arrastra la cámara para moverla y tócala para abrir la foto.
  - También puedes tomarla desde la pestaña **Fotos** de arriba, que muestra todas las fotos del levantamiento, o con el botón de cámara del cuadro de medidas de un espacio.
  - En la foto, con **Medida** arrastras el lápiz de un extremo al otro de lo que mediste y escribes la medida en la casilla (2.40, o 2,40). Con **Nota** tocas y escribes un texto (enchape, sin pañete, humedad…).
  - Toca una medida para cambiarla o borrarla. Arrastra sus puntas para ajustarla o el número para correrla. Con dos dedos acercas o alejas la foto.
  - **Guardar imagen** saca la foto con las medidas dibujadas, para guardarla en Fotos o mandarla por WhatsApp.
  - Las fotos salen al final del PDF, una por hoja con sus medidas, y van dentro del archivo de **Guardar**.
- **Mover:** arrastra cualquier cosa. En un espacio seleccionado, los puntos de las esquinas cambian su forma, y si arrastras un muro lo corres completo.
- **Alzados:** arrastra puertas y ventanas para cambiar la altura, el antepecho y la posición. Arrastra la esquina de arriba de un muro para cambiar su altura.
- **Escribir a mano:** en cualquier casilla de medida puedes escribir el número con el lápiz y el iPad lo convierte en texto (Garabatear / Scribble).
- **Cuadro de medidas flotante** (queda medio transparente mientras no lo usas; al tocarlo se ve completo): al tocar cualquier muro, puerta, ventana, elemento, losa, escalera, cubierta o espacio aparece un cuadro con sus medidas (ancho, alto, espesor, antepecho…).
  - Toca una casilla: queda vacía y escribes el número encima con el lápiz. Si no escribes nada, vuelve el valor anterior.
  - Con Enter (o al tocar otra casilla) se aplica y pasa a la siguiente.
  - Arrástralo de su barra oscura para ponerlo donde no estorbe; la app recuerda el sitio. La × lo cierra hasta que toques otro elemento y los tres puntos abren todos los datos en el panel.
- **Menú rápido del lápiz:** deja el lápiz quieto sobre el plano medio segundo (o apriétalo fuerte) y sale un menú en círculo.
  - Sobre un elemento: Medidas, Largo, Girar, Duplicar, Tipo, Puerta, Ventana, Deshacer y Eliminar, según lo que sea.
  - En un sitio vacío: cambiar de herramienta, Deshacer y Ajustar vista.
  - Desliza el lápiz hacia la opción y suéltalo, o suéltalo en el centro y toca la opción.
  - Mientras dibujas muros, cubiertas, losas, cortes o escaleras hay que sostenerlo un poco más (casi un segundo), para que no salga sin querer.
- **Borrar:** la herramienta **Borrar** (la goma, debajo de Mover).
  - Toca lo que quieras borrar.
  - O pasa el lápiz por encima de varios muros, puertas, ventanas y elementos: se marcan en rojo y se borran todos al levantar el lápiz.
  - Al borrar un muro los demás se quedan en su sitio, como en ArchiCAD.
  - Si te equivocas, ↶ deshace. Con teclado, la tecla Suprimir borra lo seleccionado.
- **Cuadro de cada herramienta:** todas las herramientas abren su cuadro flotante al tocarlas, igual que Muro. El cuadro queda medio transparente mientras no lo usas.
  - **Puerta, Ventana, Cubierta, Losa y Elemento:** los tipos salen en el cuadro en tamaño pequeño y la lista se queda abierta. ▾ la recoge.
  - **Vano:** ancho y alto de los vanos nuevos.
  - **Losa:** espesor.
  - **Escalera:** huella, contrahuella y ancho.
  - **Corte:** profundidad de vista.
  - **Daño:** tipo de daño (humedad, fisura…).
  - **Foto:** tomar o elegir la foto.
  - **Mover** y **Borrar:** qué hacer con el lápiz.
  - Todas, menos Foto y Borrar, traen el redondeo.
- **Panel de datos:** se muestra y se oculta con el botón **Panel** de arriba o con la pestaña **‹ ›** del borde derecho. Viene oculto para dejar todo el espacio al plano.

## Uso diario sin internet

- Ábrela siempre **desde el ícono**, no desde Safari.
- **Exportar:** toca **Exportar** y elige el formato. Se abre la hoja de compartir; ahí toca **Guardar en Archivos**.
  - **DXF** para AutoCAD, con plantas y alzados en capas. Los textos están a escala 1:50.
  - **PDF** en hoja carta o doble carta, con rótulo y escala.
  - **CSV** con los cuadros, para abrir en Excel.
  - **Respaldo .json** de cada proyecto.
- **Pasar archivos al computador:** desde la app Archivos, por AirDrop, cable o memoria USB-C.

## Guardar en el iPad

- Toca **Guardar**, arriba a la derecha (o Cmd + S con teclado).
- En la hoja que se abre, toca **Guardar en Archivos**, elige **En mi iPad** (o una carpeta tuya, por ejemplo "Levantamientos") y toca **Guardar**.
- El archivo queda con el nombre del proyecto, la fecha y la hora, por ejemplo `Casa_Acevedo_2026-11-07_1619.json`. Así cada vez que guardas tienes una copia nueva y no se pisa la anterior.
- **Guardar todos** (en la lista de proyectos) guarda todos tus levantamientos en un solo archivo.
- Para recuperarlos, en la lista de proyectos toca **Abrir archivo guardado…** y elige el archivo en Archivos. Sirve también para pasar los levantamientos a otro iPad o al computador.

## Cuidado con los datos

- La app guarda sola mientras trabajas, pero esa copia vive dentro de la app.
- **Si borras el ícono de la app, se borra esa copia.** Por eso toca **Guardar** al terminar cada jornada de obra.

## Cuando haya una versión nueva

1. Sube los archivos nuevos al mismo repositorio para reemplazar los anteriores (Add file → Upload files → Commit changes).
2. Espera unos 2 minutos a que GitHub publique los cambios.
3. En el iPad, con internet, abre la app desde el ícono y espera unos 10 segundos.
4. Ciérrala por completo: desliza hacia arriba desde la parte de abajo de la pantalla y quita la app de la lista.
5. Ábrela otra vez. Ya tendrás la versión nueva.

Tus proyectos no se pierden al actualizar.
