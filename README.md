# Quinza — páginas legales para GitHub Pages

Archivos independientes: index.html, privacy.html, terms.html y styles.css. No requieren instalación, JavaScript ni un proceso de compilación. No se añaden analítica, cookies, anuncios o fuentes externas al sitio.

## Estado de revisión

Los textos recogen las respuestas del responsable. Antes de publicar, confirmar si la app integra Firebase Crashlytics u otro SDK de diagnóstico. La captura del menú de Firebase no prueba si un SDK está activo. Revisar el código exportado (pubspec.yaml, inicialización y configuración de SDK) o la configuración de FlutterFlow. Si hay recopilación de diagnóstico, describir los datos, finalidad, proveedor y retención antes de publicar privacy.html. El usuario indicó que no utiliza Analytics.

Verificar que las reglas de Firestore hacen efectiva la privacidad por usuario; estas páginas no configuran ni auditan Firebase. Confirmar que Firebase Cloud Messaging corresponde al mecanismo real de notificaciones y que se pueden cumplir las solicitudes de eliminación en 15 días, incluyendo todos los documentos asociados y tokens. Si existen respaldos con retención, comunicar su periodo en la política; no se ha confirmado un periodo de respaldos.

La fecha actual de los documentos es 1 de octubre de 2026. Si se publican por primera vez otro día, ajustar fecha de entrada en vigor y última actualización, incluido el atributo datetime. Confirmar que el texto sobre menores (14 años o menos con autorización y normas aplicables para otros menores) expresa la decisión del responsable. No se ha añadido un sistema de verificación de edad o autorización en la app.

## Publicar en GitHub Pages

1. Crear un repositorio de GitHub para el sitio (público si el plan lo requiere).
2. Subir el contenido de esta carpeta a la raíz del repositorio; conservar styles.css junto a los tres HTML.
3. En Settings > Pages, seleccionar Deploy from a branch, rama main y carpeta / (root). Guardar.
4. Esperar el despliegue y abrir la URL que muestre GitHub Pages.
5. Abrir Inicio y comprobar ambos enlaces en móvil.
6. Copiar la URL pública que termine en /privacy.html para la política en Google Play Console. La de términos termina en /terms.html.
7. Para el recurso web de eliminación se puede usar la URL de /privacy.html#eliminacion. Comprobar la navegación hasta esa sección.

## Antes de Google Play

Google Play requiere una opción fácilmente visible para iniciar la eliminación desde la app y desde un recurso web. Añadir dentro de Quinza una opción claramente identificada para solicitarla; tener instrucciones únicamente en la web no completa el requisito de la app.

La política pública debe corresponder al comportamiento real de la app y a la sección Seguridad de los datos. Si se dirige a menores, revisar también la audiencia declarada y las políticas de Familias pertinentes; una autorización escrita en estos documentos no sustituye los requisitos técnicos y de la tienda.

Fuentes oficiales de verificación:
- https://support.google.com/googleplay/android-developer/answer/10144311
- https://firebase.google.com/support/privacy
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

La publicación aún no está realizada: falta acceso al repositorio de destino. Los archivos están preparados para subir a GitHub Pages.
