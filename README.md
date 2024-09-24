# Comandos CMD de Windows

## Índice

1. [Comandos Funcionales](#comandos-funcionales)
   - [Creación de un ejecutable independiente](#creación-de-un-ejecutable-independiente)
   - [Compresión y descompresión de archivos](#compresión-y-descompresión-de-archivos)
2. [Comandos Útiles](#comandos-útiles)
   - [Ver contraseña de WiFi](#ver-contraseña-de-wifi)
   - [Monitoreo de recursos del sistema](#monitoreo-de-recursos-del-sistema)
3. [Comandos Interesantes](#comandos-interesantes)
   - [Mostrar la película de Star Wars](#mostrar-la-película-de-star-wars)
   - [Calculadora científica](#calculadora-científica)
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

## Comandos Interesantes

### Mostrar la película de Star Wars

Este comando te permitirá ver la película de Star Wars completa desde la terminal:

```
telnet towel.blinkenlights.nl
```

Al ejecutar este comando, la terminal mostrará la película de Star Wars ASCII art, proporcionando una experiencia única y divertida.

### Calculadora científica

Windows también incluye una calculadora científica que puedes acceder desde la terminal:

```
calc
```

Al ejecutar este comando, se abrirá la calculadora científica de Windows, donde podrás realizar operaciones matemáticas avanzadas.

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
