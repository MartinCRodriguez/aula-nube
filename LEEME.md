# Aula Nube — Railway

Proyecto para la materia **Conceptualización de servicios en la nube**.

- Alumno: Martin Curiel Rodriguez
- Código: 222958593
- Correo: martincurielrodriguez@gmail.com
- Interfaz: HTML5 y CSS3
- Servidor: JavaScript con Node.js, sin dependencias externas
- Plataforma prevista: Railway

Estado: archivos preparados y servidor probado localmente. El despliegue en Railway y su URL pública están pendientes.

## Contenido

| Archivo | Función |
|---|---|
| package.json | Define Node.js y el comando npm start |
| package-lock.json | Archivo de bloqueo para la instalación con npm |
| server.js | Sirve la página, los estilos y las imágenes |
| public/index.html | Página completa y datos de identificación |
| public/styles.css | Diseño adaptable e imagen de fondo |
| public/assets/logo.svg | Imagen del logo |
| public/assets/fondo.svg | Imagen de fondo |

## Requisitos de la actividad

- Todo el contenido visible está dentro de `div.contenedor`.
- El encabezado es un `div` con `id="header"`.
- La imagen del logo está a la izquierda del encabezado.
- El body contiene un enlace a Nuestro planeta en Netflix, con acceso a su ficha y tráileres.
- El footer incluye curso, nombre completo, código y correo.
- El fondo utiliza una imagen SVG incluida en el proyecto.

La reproducción del documental completo en Netflix puede requerir una cuenta y suscripción. La página académica contiene el enlace externo; no aloja ni reproduce directamente ese contenido.

## Prueba en tu equipo

Requiere Node.js 22 o 24. Abre una terminal dentro de la carpeta que contiene package.json y ejecuta:

```bash
npm start
```

Abre http://localhost:3000 . Detén el servidor con Ctrl+C.

No es necesario instalar paquetes de terceros. Railway puede ejecutar la instalación estándar de npm utilizando el archivo de bloqueo incluido.

## Subir a GitHub

1. Descomprime el ZIP.
2. Crea un repositorio llamado `aula-nube-railway`, o utiliza tu repositorio de esta actividad.
3. Selecciona **Add file > Upload files**.
4. Sube el CONTENIDO de la carpeta `aula-nube-railway`: `package.json`, `package-lock.json`, `server.js`, `LEEME.md` y la carpeta `public` completa. Incluye `.gitignore` si es visible.
5. Pulsa **Commit changes**.

IMPORTANTE: `package.json` debe quedar en la raíz del repositorio, al mismo nivel que `server.js` y la carpeta `public`. No subas únicamente el ZIP. Si antes subiste la versión para Render, añade los nuevos archivos en la raíz y sustituye la carpeta `public` por esta versión.

## Despliegue en Railway

Procedimiento basado en el recurso oficial **Getting Started on Railway**, que actualmente redirige a **Quick Start Tutorial**:

https://docs.railway.app/getting-started
https://docs.railway.com/quick-start

1. Inicia sesión en https://railway.com y vincula tu cuenta de GitHub.
2. Desde el panel, selecciona **New Project** y la opción para desplegar desde un repositorio de GitHub.
3. Autoriza el acceso al repositorio de esta actividad y selecciónalo.
4. Selecciona **Deploy Now** si aparece. Railway analizará el proyecto Node.js y comenzará el despliegue.
5. Si solicita configuración, utiliza estos valores:

| Campo | Valor |
|---|---|
| Root Directory | Raíz del repositorio; dejar el valor predeterminado |
| Build Command | Automático; este proyecto no necesita compilación |
| Start Command | npm start |
| Variables | No se necesitan variables manuales para esta aplicación |

El servidor escucha en `0.0.0.0` y utiliza la variable `PORT` que proporciona Railway. En tu equipo utiliza el puerto 3000 de forma predeterminada.

6. Revisa los registros hasta que el servicio esté ejecutándose sin errores.
7. En la configuración del servicio, busca la sección de red pública (**Networking / Public Networking**) y pulsa **Generate Domain**. Si pide un puerto de destino, usa el puerto real mostrado en los registros del servidor; Railway proporciona `PORT` automáticamente.
8. Abre la URL HTTPS generada. Comprueba la página, el logo, el fondo, el footer, los enlaces internos y el enlace de Netflix.
9. Prueba la URL desde una ventana privada para verificar que el asesor pueda acceder al sitio.
10. Guarda la URL real y las capturas del despliegue para el documento de entrega.

La disponibilidad del despliegue depende del plan, los créditos y la verificación de tu cuenta. Revisa las condiciones que muestre Railway antes de aceptar un cobro; no se presupone alojamiento gratuito permanente.

## Documento de entrega

El PDF final se completa después del despliegue, con:

1. Portada con la materia, actividad y datos del alumno.
2. URL HTTPS real de la aplicación, como enlace pulsable.
3. Descripción del sitio y del uso de Node.js para servir HTML y CSS en Railway.
4. Procedimiento realmente realizado y configuración utilizada.
5. Capturas del despliegue y de la página publicada con su URL visible.
6. Código copiado, si lo solicita el asesor.
7. Referencias oficiales.

Este ZIP contiene los archivos de trabajo. No sustituye al PDF solicitado en el buzón ni constituye evidencia de que la página ya fue publicada.

## Referencias

Documentación consultada el 28 de octubre de 2026:

- Railway. *Quick Start Tutorial* (recurso anteriormente denominado *Getting Started on Railway*). https://docs.railway.com/quick-start
- Railway. *No Start Command Could be Found*. https://docs.railway.com/deployments/troubleshooting/no-start-command-could-be-found
- Railway. *Application Failed to Respond*. https://docs.railway.com/networking/troubleshooting/application-failed-to-respond
- Netflix. *Nuestro planeta*. https://www.netflix.com/mx/title/80049832

La fecha de consulta del 7 de agosto de 2023 pertenece a la referencia original proporcionada en el curso; no corresponde a la consulta realizada para este proyecto.
