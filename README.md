# Comandos CMD de Windows

## Índice

1. [Comandos Funcionales](#comandos-funcionales)
2. [Comandos Útiles](#comandos-útiles)
3. [Comandos Interesantes](#comandos-interesantes)
4. [Comandos Divertidos](#comandos-divertidos)

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

## Comandos Interesantes

(No se encontraron comandos interesantes en el documento original)

## Comandos Divertidos

Estos comandos te mostrarán animaciones divertidas en la terminal:

- Ver un pájaro bailando:
  ```
  curl parrot.live
  ```
- Ver el baile de Rick:
  ```
  curl ascii.live/rick
  ```
- Ver a Forrest Gump corriendo:
  ```
  curl ascii.live/forrest
  ```
