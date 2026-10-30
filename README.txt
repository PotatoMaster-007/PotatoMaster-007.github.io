SITIO ESTÁTICO PARA LA CONFIGURACIÓN PERSONAL DE RCLONE + GOOGLE DRIVE

ARCHIVOS
- index.html    Página principal de la aplicación.
- privacy.html  Política de privacidad detallada.
- styles.css    Estilos compartidos y diseño adaptable a móviles.

PUBLICACIÓN EN GITHUB PAGES
1. Descarga y descomprime este paquete.
2. Copia los tres archivos a la raíz del repositorio que publica tu sitio:
   potatomaster-007.github.io
3. Sustituye el index.html anterior. Puedes retirar los archivos de ejemplos XML/CSS/JSON que ya no quieras mostrar.
4. En GitHub, abre Settings > Pages y comprueba que Pages publica desde la rama y carpeta que contienen estos archivos (por ejemplo, main / root).
5. Cuando la publicación termine, comprueba que ambas direcciones se abren sin iniciar sesión:
   Página principal: https://potatomaster-007.github.io/
   Política:         https://potatomaster-007.github.io/privacy.html

CONFIGURACIÓN EN GOOGLE CLOUD
- Nombre de la aplicación: rclone
- Página principal de la aplicación: https://potatomaster-007.github.io/
- Enlace a la política de privacidad: https://potatomaster-007.github.io/privacy.html

IMPORTANTE SOBRE EL ALCANCE OAUTH
La política explica que los permisos reales dependen del alcance configurado. La opción habitual de rclone es `drive` (acceso a los archivos de Drive, salvo la carpeta de datos de aplicaciones). Si eliges otro alcance, revisa que la descripción de los permisos en Google Cloud coincida con lo que realmente solicitas en rclone.

IMPORTANTE SOBRE LA VERIFICACIÓN DE GOOGLE
Este paquete corrige el contenido de las páginas y la correspondencia del nombre, pero no demuestra por sí solo la propiedad del dominio. Google indica que una verificación formal de marca requiere un dominio verificado bajo tu control y advierte sobre subdominios de plataformas de terceros que no puedas verificar. Por ello, Google todavía podría rechazar `github.io` por la propiedad del sitio, aunque las páginas estén bien configuradas.

La documentación de rclone indica que GitHub Pages puede servir para completar los campos de página principal y política de privacidad y publicar una aplicación personal. Si Google exige verificar formalmente el dominio, la solución más fiable es conectar un dominio personalizado que controles a GitHub Pages y verificarlo en Google Search Console.

Para una aplicación de uso exclusivamente personal, consulta la exención de verificación descrita en la documentación de rclone. Publicar la aplicación para uso personal no equivale a obtener la verificación formal de marca; es posible que Google siga mostrando una advertencia de aplicación no verificada durante la autorización.

ANTES DE PUBLICAR
El contenido está redactado para el escenario descrito: una sola persona usa rclone localmente con su propia cuenta de Google Drive, sin ofrecer el servicio a terceros ni operar un backend propio. Si tu uso real cambia (por ejemplo, habilitas a otras personas, añades un servidor o transfieres datos a otros destinos), actualiza la política para reflejarlo.
