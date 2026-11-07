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
- **Medida exacta:** toca la cota de un muro, escribe la medida y toca OK. Los muros de al lado se acomodan solos.
- **Puerta, Ventana y Vano:** toca el muro donde va y arrástralo a su sitio. Los puntos de los extremos cambian el ancho.
- **Cubierta:** arrastra con el lápiz de una esquina a la otra para dibujarla. Si solo tocas dentro de un espacio, se crea encima de él con un alero de 0.50 m.
  - En la barra de arriba eliges el tipo: Plana, 1 agua, 2 aguas o 4 aguas.
  - Tocando el % cambias la pendiente; con **Girar caída** cambias hacia dónde corre el agua.
  - Con **Mover:** arrastra la cubierta, estira sus esquinas o gírala con el círculo.
  - En **Datos** pones la altura del alero o de la cumbrera (la pendiente se recalcula sola), el material y el estado.
  - El PDF y el DXF traen una hoja de **planta de cubiertas**, y el cuadro muestra el área en planta y el área inclinada.
- **Elemento** (columnas, vigas, aparatos, tanques…): elige el elemento, tócalo en el plano y arrástralo a donde quieras. Cerca de una esquina o de un muro se pega solo.
  - El círculo de arriba lo gira.
  - El punto de la esquina cambia su tamaño.
- **Mover:** arrastra cualquier cosa. En un espacio seleccionado, los puntos de las esquinas cambian su forma, y si arrastras un muro lo corres completo.
- **Alzados:** arrastra puertas y ventanas para cambiar la altura, el antepecho y la posición. Arrastra la esquina de arriba de un muro para cambiar su altura.
- **Escribir a mano:** en cualquier casilla de medida puedes escribir el número con el lápiz y el iPad lo convierte en texto (Garabatear / Scribble).
- **Datos:** el botón de arriba abre el panel con toda la información del elemento seleccionado.

## Uso diario sin internet

- Ábrela siempre **desde el ícono**, no desde Safari.
- **Exportar:** toca **Exportar** y elige el formato. Se abre la hoja de compartir; ahí toca **Guardar en Archivos**.
  - **DXF** para AutoCAD, con plantas y alzados en capas. Los textos están a escala 1:50.
  - **PDF** en hoja carta o doble carta, con rótulo y escala.
  - **CSV** con los cuadros, para abrir en Excel.
  - **Respaldo .json** de cada proyecto.
- **Pasar archivos al computador:** desde la app Archivos, por AirDrop, cable o memoria USB-C.

## Cuidado con los datos

- Los proyectos viven **solo en este iPad**.
- **Si borras el ícono de la app, se borran los proyectos.** Exporta antes el respaldo .json de cada uno.
- Exporta el respaldo .json de cada obra al terminarla y guárdalo en el computador.
- Para abrir un respaldo en otro iPad: Proyecto ▾ → **Importar respaldo…**

## Cuando haya una versión nueva

1. Sube los archivos nuevos al mismo repositorio para reemplazar los anteriores (Add file → Upload files → Commit changes).
2. Espera unos 2 minutos a que GitHub publique los cambios.
3. En el iPad, con internet, abre la app desde el ícono y espera unos 10 segundos.
4. Ciérrala por completo: desliza hacia arriba desde la parte de abajo de la pantalla y quita la app de la lista.
5. Ábrela otra vez. Ya tendrás la versión nueva.

Tus proyectos no se pierden al actualizar.
