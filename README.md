# Scout para Windows

Buscador local de aplicaciones, archivos y comandos. distribución de instaladores, notas y metadatos de actualizacion.

## Instalar o actualizar

La version disponible es **0.13.12 alpha** para Windows x64, en el [canal preliminar](https://github.com/Alexis12240/Scout-releases/releases/tag/v0.13.12-alpha.20261116).

1. Descarga `Scout-0.13.12-alpha.20261116-win-x64.zip` desde los activos de esa version.
2. Extrae **todo** el ZIP a una carpeta nueva y abre `Scout.Setup.exe`.
3. Si Scout esta abierto, cierralo desde **Salir de Scout**; la X solo lo oculta. En 0.13.12 o posterior tambien existe `Scout.exe --exit` para solicitar el cierre normal.
4. Sigue el panel. Conserva indices y preferencias existentes. La preparacion integrada del teclado y NTFS puede solicitar UAC.

El paquete incluye los modelos y motores fijados para busqueda semantica y multimedia; no requiere cuenta de GitHub. La indexacion inicial puede consumir recursos y no equivale a un indice ya terminado. Las licencias de terceros estan incluidas en `payload/licenses` y en sus distribuciones de runtime.

Esta preliminar **no tiene firma Authenticode**; Windows puede mostrar una advertencia de editor. `SHA256SUMS.txt` permite comprobar la descarga. La firma del canal autentica los metadatos y los hashes, no es un certificado de Windows.

## Actualizaciones

Scout verifica los canales `channels/preview.json` y `channels/stable.json` con su clave publica fijada. Las versiones alpha consultan Preview. Stable aun no ofrece una version final.

Se mantiene **Avisar y pedirme actualizar** o consulta manual. El cliente abre las notas por accion del usuario; no descarga ni ejecuta instaladores silenciosamente. La instalacion usa el panel transaccional con verificacion y recuperacion.

`publisher-key.spki` es la clave publica RSA-PSS/SHA-256. La clave privada no se almacena aqui. Los paquetes no incluyen perfiles, consultas, credenciales ni indices personales.

## Estado de la preliminar

Incluye mejoras de busqueda, iconos genericos, arranque, foco, almacenamiento progresivo, mascota y diagnostico. Se validaron 597 comprobaciones de contratos/interfaz/cache con perfiles aislados. Sigue pendiente confirmar nuevamente el primer acceso tras un reinicio completo del equipo y observar estabilidad prolongada. No se declara CORE01 terminado ni una reduccion porcentual de RAM.
