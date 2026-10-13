# FUNDALID Campus V2

Sitio demostrativo estático y responsive creado en HTML/CSS/JS. No requiere npm ni compilación.

## Módulos
Campus/estudiantes, cursos asincrónicos, eventos y FLS2026, networking (conexiones, proyectos, alianzas, productos propios), partners, sponsors, egresados, postulación facilitador/voluntario, Fundalid TV, franja de convenios y chatbot FAQ demostrativo.

## Limitaciones
- Cursos y sus descripciones son **ejemplos**, no ofertas publicadas por FUNDALID.
- Accesos por perfil son demostrativos; **sin** registro, contraseñas, autenticación ni gestión real de permisos. Configurar Cognito.
- Chatbot es FAQ local y no utiliza IA ni envía mensajes a servidores.
- TV en vivo, formularios de postulación, eventos, biblioteca de videos/PDF y convenios necesitan contenido, backend y enlaces oficiales.
- Identidad cromática aproximada basada en capturas, no en manual de marca. El logotipo usado es tipográfico, no el logo original.

## Publicar desde GitHub en Amplify
1. Copiar los archivos a la raíz del repositorio `fundalid`, reemplazando los anteriores.
2. `git add . && git commit -m "Rediseño completo campus FUNDALID V2" && git push origin main`
3. Amplify conectado al repositorio desplegará la rama main. Usar `amplify.yml` incluido o configurar el directorio de publicación como `/`.

## Publicación manual
Cargar el ZIP `fundalid-v2-deploy.zip` por despliegue manual en Amplify Hosting. El ZIP tiene `index.html`, `styles.css`, `app.js` en su raíz.

## Próximas fases sugeridas
Cognito (roles y grupos), API Gateway/Lambda, persistencia, S3/CloudFront con acceso privado, LMS, publicación de cursos, chat con Bedrock y live streaming con Amazon IVS.
