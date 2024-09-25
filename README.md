# Comandos CMD de Windows

## Índice

1. [Comandos Funcionales](#comandos-funcionales)
   - [Creación de un ejecutable independiente](#creación-de-un-ejecutable-independiente)
   - [Compresión y descompresión de archivos](#compresión-y-descompresión-de-archivos)
   - [Combinar una imagen y un archivo](#combinar-una-imagen-y-un-archivo)
   - [Crear una copia de seguridad del registro](#crear-una-copia-de-seguridad-del-registro)
2. [Comandos Útiles](#comandos-útiles)
   - [Ver contraseña de WiFi](#ver-contraseña-de-wifi)
   - [Monitoreo de recursos del sistema](#monitoreo-de-recursos-del-sistema)
   - [Desbloquear una cuenta de usuario](#desbloquear-una-cuenta-de-usuario)
   - [Enviar mensaje a usuarios conectados](#enviar-mensaje-a-usuarios-conectados)
3. [Comandos Interesantes](#comandos-interesantes)
   - [Mostrar la película de Star Wars](#mostrar-la-película-de-star-wars)
4. [Comandos Divertidos](#comandos-divertidos)
   - [Ver un pájaro bailando](#ver-un-pájaro-bailando)
   - [Ver el baile de Rick](#ver-el-baile-de-rick)
   - [Ver a Forrest Gump corriendo](#ver-a-forrest-gump-corriendo)

## Comandos Funcionales

### Creación de un ejecutable independiente

Para crear un ejecutable independiente que incluya Python y todas las dependencias necesarias, puedes seguir estos pasos usando PyInstaller:

1. Instala PyInstaller:
   ```
   pip install pyinstaller
   ```
2. Navega hasta el directorio donde se encuentra tu script principal (script que quieras hacer ejecutable).
3. Ejecuta el siguiente comando para crear el ejecutable:
   ```
   pyinstaller --onefile --name NombreFinalScript el_script.py
   ```
4. PyInstaller creará una carpeta llamada `dist` que contendrá tu ejecutable `NombreFinalScript.exe`.
5. Ahora puedes distribuir este archivo `.exe` a otros usuarios, y podrán ejecutarlo sin necesidad de instalar Python o las dependencias por separado.

**Nota:** El archivo ejecutable resultante será significativamente más grande que el script original, ya que incluirá Python y todas las dependencias necesarias.

"Algunos antivirus pueden marcar erróneamente los ejecutables creados con PyInstaller como maliciosos. Esto es un falso positivo común."

### Compresión y descompresión de archivos

Windows dispone de herramientas integradas para comprimir y descomprimir archivos. Algunos de los comandos más útiles son:

- Comprimir archivos en un archivo ZIP:
  ```
  zip archivo.zip archivo1.txt archivo2.txt
  ```
- Descomprimir un archivo ZIP:
  ```
  unzip archivo.zip
  ```
- Comprimir archivos en un archivo RAR (requiere software de terceros):
  ```
  rar a archivo.rar archivo1.txt archivo2.txt
  ```
- Descomprimir un archivo RAR (requiere software de terceros):
  ```
  unrar x archivo.rar
  ```

### Combinar una imagen y un archivo

Puedes combinar una imagen y un archivo de forma que el archivo quede "oculto" dentro de la imagen. Esto puede ser útil para enviar archivos de forma más discreta o esconderlos visualmente. El comando para hacer esto es:

```
copy /b imagen.png + archivo.rar archivo_combinado.png
```

Reemplaza `imagen.png` con el nombre de tu imagen, `archivo.rar` con el nombre del archivo que quieres ocultar, y `archivo_combinado.png` con el nombre que quieres darle al archivo resultante. Cuando abras `archivo_combinado.png`, podrás extraer el archivo oculto.

### Crear una copia de seguridad del registro

Puedes crear una copia de seguridad del registro de Windows utilizando el siguiente comando:

```
reg export HKEY_CURRENT_USER backup_registro.reg
```

Este comando exportará todo el registro de usuario actual a un archivo llamado `backup_registro.reg`. Posteriormente, podrás importar este archivo para restaurar la configuración del registro en caso de ser necesario.

## Comandos Útiles

### Ver contraseña de WiFi

Estos comandos te permitirán ver la contraseña de la red WiFi a la que estás conectado:

1. Muestra la lista de redes a las que has estado o estás conectado:
   ```
   netsh wlan show profile
   ```
2. Para ver la contraseña de una red específica, reemplaza `"nombre"` por el nombre de la red que te interesa:
   ```
   netsh wlan show profile name="nombre" key=clear
   ```

### Monitoreo de recursos del sistema

Estos comandos te permiten monitorear el uso de recursos del sistema, como CPU, memoria y disco:

- Muestra el uso de CPU:
  ```
  wmic cpu get loadpercentage
  ```
- Muestra el uso de memoria RAM:
  ```
  wmic memphysical get MaxMemoryModuleSize, MemoryModules, Speed
  wmic memphysical get Speed, MaxMemoryModuleSize, MemoryModules
  ```
- Muestra el uso de disco:
  ```
  wmic logicaldisk get Size, FreeSpace, DeviceID
  ```

### Desbloquear una cuenta de usuario

Puedes usar este comando para desbloquear una cuenta de usuario que haya sido bloqueada, por ejemplo, debido a intentos fallidos de inicio de sesión:

```
net user usuario /active:yes
```

Reemplaza `usuario` por el nombre de la cuenta que deseas desbloquear. Ten en cuenta que este comando debe ser utilizado con precaución, ya que podría permitir que usuarios no autorizados accedan a cuentas que han sido bloqueadas por razones de seguridad.

### Enviar mensaje a usuarios conectados

Este comando te permite enviar un mensaje de texto a otros usuarios que estén conectados al mismo sistema Windows:

```
msg usuario Hola, este es un mensaje para ti.
```

Reemplaza `usuario` por el nombre de la cuenta a la que deseas enviar el mensaje. Puedes ver la lista de usuarios conectados utilizando el comando `query user`.

Usa este comando con prudencia, ya que podría utilizarse para enviar mensajes molestos o no deseados a otros usuarios.

## Comandos Interesantes

### Mostrar la película de Star Wars

Este comando te permitirá ver la película de Star Wars completa desde la terminal:

```
telnet towel.blinkenlights.nl
```

Al ejecutar este comando, la terminal mostrará la película de Star Wars ASCII art, proporcionando una experiencia única y divertida.

## Comandos Divertidos

### Ver un pájaro bailando

```
curl parrot.live
```

Este comando mostrará una animación de un pájaro bailando en la terminal.

### Ver el baile de Rick

```
curl ascii.live/rick
```

Este comando mostrará una animación del famoso baile de Rick Astley en la terminal.

### Ver a Forrest Gump corriendo

```
curl ascii.live/forrest
```

Este comando mostrará una animación de Forrest Gump corriendo en la terminal.

