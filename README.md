# Pasos a seguir para usar el administrador de Proyecto Horus en Linux o MacOS

- Paso 1: Descargar el software portable de:
    https://www.proyectohorus.com.ar/descargas/windows/portable.zip
    
    Podes hacerlo tanto haciendo click en el link o desde terminal (Paso 2) usando wget:
    
    sudo wget https://www.proyectohorus.com.ar/descargas/windows/portable.zip

- Paso 2: Entra en el terminal (Solo usuarios Linux)

- Paso 3: Actualiza tu Linux (Solo usuarios Linux)

    sudo apt-get update
    sudo apt-get upgrade
    
- Paso 4 Descomprime el contenido en la ubicación que quieras.
    
    Para este paso deberas tener instalado Zip o RAR.
    
    En caso de Linux Debian o Ubuntu:
    
        sudo apt install unzip
    
    En Centos o Fedora:
        
        sudo yum install unzip
        
    En MacOS:
    
        Descargando la app de https://www.winrar.es/descargas
    
  y por ultimo:
    
        sudo unzip portable.zip
        
- Paso 5: Instala Mono

      En Linux Debian o Ubuntu:
      
        sudo apt-get install mono-complete
        
      En Centos o Fedora:
      
        rpmkeys --import "http://pool.sks-keyservers.net/pks/lookup?op=get&search=0x3fa7e0328081bff6a14da29aa6a19b38d3d831ef" 
        su -c 'curl https://download.mono-project.com/repo/centos8-stable.repo | tee /etc/yum.repos.d/mono-centos8-stable.repo'
    
        yum install mono-devel

    En MacOS instalando:
    
        https://www.mono-project.com/download/stable/#download-mac

- Paso 6: Ejecuta la interfaz de Horus
    
        En linux ejecutando:
            sudo mono Proyecto\ Horus.exe

        En MacOS:
            Haciendo doble click sobre "Proyecto Horus.exe"

Es todo, simple y rápido!

Nota: La función de prueba en vivo puede no funcionar en algunas versiones de MacOS o Linux
