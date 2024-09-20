
<div style="background-image: url(https://media3.giphy.com/media/wwg1suUiTbCY8H8vIA/giphy.gif?cid=ecf05e47hfu84pmh8vk2mo5wohm7vxo4hcx1gu3ye1664zcy&ep=v1_gifs_search&rid=giphy.gif&ct=g); display: flex; justify-content: center;">

# CMD-Windows-Comands from [Sicer Andres Brito Gutierrez 👨‍💻](https://github.com/SicerBrito)
</div>

## Índice 📖
Estos son algunos ```Comandos``` cuanto menos ```Interesantes```, ```Útiles```, ```Divertidos``` y ```Curiosos``` del ```CMD de Windows``` 💻. Espero que los disfruten y les sean útiles dependiendo de lo que necesiten o quieran realizar.

- [Comandos](#comandos) 📄
    - [Curiosos](#útiles) ⁉
    - [Útiles](#terminal) 🛠
        <!-- - [Estructura Base](#estructura-base) 🚧
        - [Referencias](#referencias) 🔗 -->
    - [Interesantes](#interesantes) 🔍
        <!-- - [Instalación de Paquetes](#instalación-de-paquetes) ⏬
            - [Dominio](#dominio) 📂
            - [Persistencia](#persistencia) 📂
            - [API](#api) 📂
        - [Migraciones](#migraciones) ✈️
            - [Crear](#crear) 🔧
            - [Actualizar](#actualizar) 🔧
        - [Visualización de posibles errores](#visualización-de-posibles-errores) ⁉️ -->
    - [Divertidos](#divertidos) 🤡


---

 - ## ```Comandos```

    - ### ```Funcionales```
       - ```Creación de un ejecutable independiente```

        Para crear un ejecutable independiente que incluya Python y todas las dependencias necesarias, seguiremos estos pasos usando PyInstaller:
      
      1. Instala PyInstaller:
          ```
          pip install pyinstaller
          ```
      2. Navega hasta el directorio donde se encuentra tu script principal (script que quieras hacer ejecutable).
      3. Ejecuta el siguiente comando para crear el ejecutable:
          ```
          pyinstaller --onefile --name NombreFinalScript el_script.py
          ```
      4. PyInstaller creará una carpeta llamada dist que contendrá tu ejecutable NombreFinalScript.exe.
      5. Ahora puedes distribuir este archivo .exe a otros usuarios, y podrán ejecutarlo sin necesidad de instalar Python o las dependencias por separado.

      **Nota: ** El archivo ejecutable resultante será significativamente más grande que el script original, ya que incluirá Python y todas las dependencias necesarias.
      
      "Algunos antivirus pueden marcar erróneamente los ejecutables creados con PyInstaller como maliciosos. Esto es un falso positivo común."



    - ### ```Curiosos```
    - ### ```Útiles```
        Comandos para ver la contraseña del WIFI con conexión Inalámbrica.

        - Este comando muestra la lista de redes a las que has estado o estas conectado en estos momentos

            ```
            netsh wlan show profile
            ```

        - Este comando nos permite ver la configuración de la red que elijamos, solo de debe cambiar "nombre" por el nombre de alguna red mostrada en el comando anterior
        
            ```
            netsh wlan show profile name=nombre key=clear
            ```

    - ### ```Interesantes```
    - ### ```Divertidos```
      
        - Este ```comando``` nos permite ver a un pajarito bailando en la ```Terminal```
    
        ```
        curl parrot.live
        ```
        
       - Este ```comando``` nos permite ver el baile de Rick en la ```Terminal```
    
        ```
        curl ascii.live/rick
        ```
        
       - Este ```comando``` nos permite ver a Forrest correr en la ```Terminal```
    
        ```
        curl ascii.live/forrest
        ```     
