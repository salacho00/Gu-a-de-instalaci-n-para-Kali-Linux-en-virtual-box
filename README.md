# Guia de instalacion para kali linux en virtual box

## 🧩 Requisitos previos
- **Tener (Windows/Mac/Linux), en esta instalacion usaremos windows**
- **Tener instalado el oracle virtual box, si no lo tienes descargalo aqui: https:** **https://www.virtualbox.org/wiki/Downloads**
- **Mínimo 20GB de espacio, 4GB RAM recomendado**

## Instalacion de la ISO de kali linux

dirigete a esta URL: **https://www.kali.org/get-kali/#kali-platforms**

Veras algo como esto, vamos a darle al que dice **installer images**
<img width="1105" height="466" alt="Captura de pantalla 2025-11-27 092405" src="https://github.com/user-attachments/assets/16366301-eea8-447c-b7a8-6fd7c3ca0670" />

Una vez le diste click, descarga esta que te muestro en imagen:
<img width="1432" height="825" alt="Captura de pantalla 2025-11-27 181044" src="https://github.com/user-attachments/assets/4435438e-44b4-4703-8002-79218abfea6c" />

Una vez ya descargada no hay que moverle nada mas.

## Configuraciones en Oracle VirtualBox
Abrimos la maquina virtual de oracle y nos aparecera algo asi: 

<img width="1241" height="553" alt="Captura de pantalla 2025-11-27 181345" src="https://github.com/user-attachments/assets/31af5ced-191c-44aa-b219-c2ebc9ee6cf6" />
le damos click al boton "nuevo"


Y te aparecera algo asi: 
<img width="991" height="693" alt="image" src="https://github.com/user-attachments/assets/05bf9e0b-9101-4bd3-8c0c-830697d59250" />

- En el nombre pon el que tu quieras, en este caso pondre kali linux
- El VM folder dejalo tal como te aparece a ti
- En la ISO image pon la ruta en donde esta el archivo
- En OS pon Linux (se cambia automaticamente al detectar la ISO)
- En OS Distribution pon Debian
- En OS version pon el de 64 - bit

  <img width="981" height="680" alt="Captura de pantalla 2025-11-27 182204" src="https://github.com/user-attachments/assets/4eb533c6-06ba-405a-adc1-12af3a9df775" />
La segunda flecha la ignoramos y la dejamos en blanco (esto es para instalarlo automaticamente, pero nosotros lo haremos manualmente)

En la tercera flecha pondremos las CPU y la memoria que va a usar nuestra maquina virtual, en este caso le pondremos 4gb de ram y 2 CPU, con esto va a ir fluido
<img width="991" height="683" alt="Captura de pantalla 2025-11-27 182357" src="https://github.com/user-attachments/assets/0a9ed1c4-4429-43d5-872a-de9335347626" />

En la cuarta flecha pondremos la cantidad de almacenamiento que va a tener nuestra maquina virtual, en este caso le pondre 30gb
<img width="988" height="685" alt="Captura de pantalla 2025-11-27 182829" src="https://github.com/user-attachments/assets/c0e9bda6-d967-4121-a0c4-d4bc84f1b43e" />
**importante, seleccionar la opcion que dice "create a new virtual hard disk"**

y ya con esto le daremos al boton de **"Terminar"**

## Configuracion kali linux
**HAY QUE TENER EN CUENTA QUE ENTRE CADA CONFIGURACION ECHA PUEDEN HABER TIEMPOS DE CARGA EN LOS QUE LINUX ESTE DESCARGANDO ALGO**

Una vez ya le allas dado a terminar te aparecera algo asi:

<img width="305" height="275" alt="Captura de pantalla 2025-11-27 183202" src="https://github.com/user-attachments/assets/554b42b5-d560-4bf1-b11b-545969789f10" />
esta algo borrosa pero debes deskizarte entre opciones con las flechitas y selecciona **"Graphical install"** (la primera o segunda opción, es la más fácil de usar) con el **ENTER**

A continuacion te va a pedir el lenguaje, tu region y en que idioma esta tu teclado 
**Recuerda que para seleccionar una opcion te mueves con las flechitas y para aceptar es con el boton ENTER**

- Lo siguiente que te pedira va a ser el nombre de la maquina como tal, puedes ponerle de nombre kali o el que tu quieras

- En el nombre del dominio puedes dejarlo vacio, no importa mucho 

- **Luego te pedira el nombre completo del usuario(ESTO NO ES EL USERNAME)**

- Despues te pedira ahora si el username para el ingreso

- Y despues te pedira una contraseña

Llegaras a una pantalla que preguntara sobre la particion de discos
**Guiado - utilizar todo el disco** ← Selecciona esta opcion

Al darle al boton de continuar debe aparecer el disco virtual que creamos **(debería aparecer algo como "VBOX HARDDISK" de 30 GB)**, selecciona ese y dale a continuar

Te preguntará si quieres "Todos los ficheros en una partición" ← Selecciona esta opción

 Luego te mostrará un resumen, busca la opción "Finalizar el particionado y escribir los cambios en el disco"

 Te preguntará "¿Escribir los cambios en los discos?" → Selecciona "Sí" y Continuar

### llegamos a la seleccion de programas
<img width="795" height="708" alt="Captura de pantalla 2025-11-27 100335" src="https://github.com/user-attachments/assets/5a3eb72a-5369-44a1-9884-74d468fceb37" />

Pon las opciones marcadas en la imagen y dale a continuar.

Aqui empezara a descargar todo, puede tardar entre 10-30 minutos, tambien depende del internet que tengas

En algun momento te preguntara si deseas descargar el cargador de arranque GRUB, debes responder **Si**

Despues te preguntara en donde lo quieres descargar, ve al que diga **"/dev/sda"** (disco principal), **si despues del /dev/sda ves mas cosas, no importa, selecciona ese**

**DESPUES DE TODO ESTO DEBERIA HABER TERMINADO LA INSTALACION**
Dale al continuar y la maquina se reiniciara automaticamente

Al principio apareceran algunos codigos, no te preocupes, es normal, dejalo que ejecute y no presiones nada.

Una vez ya alla cargado todo, te debe aparecer el login del Kali linux
<img width="675" height="348" alt="image" src="https://github.com/user-attachments/assets/8faf3caf-ebbe-4fa9-a7bb-47e68ee9673f" />

Ingresa el username y la contraseña que le asignamos anteriormente en la configuracion 

## CERRAR CORRECTAMENTE LA MAQUINA VIRTUAL

ya tenemos el kali linux preparado para hacer lo que quieras 
<img width="633" height="342" alt="image" src="https://github.com/user-attachments/assets/7159739a-dfdb-452c-8fb0-d48a37450f2b" />

### Como cerrar la maquina virtual:
para poder apagar la maquina debes darle al boton de la derecha superior, el mas cerca a la esquina, una vez que le des ahi, aparecera esta ventana
<img width="1270" height="893" alt="Captura de pantalla 2025-11-27 103210" src="https://github.com/user-attachments/assets/9d767f83-29c4-4705-a23c-07a2bc1c013c" />
 debes darle al que dice **Apagar**, de esa forma la maquina se cerrara correctamente y sin problemas 

### Como elimino una maquina virtual 
para eliminar una maquina virtual, nos vamos a la ventana del virtual box, desplegamos la lista de todas las maquinas que tenemos y le damos click derecho a la que queremos eliminar.
luego te aparecera una lista de opciones con la maquina y tu le das al boton de eliminar y despues de aparecera una pequeña ventana como muestra la imagen:
<img width="1185" height="946" alt="Captura de pantalla 2025-11-27 103809" src="https://github.com/user-attachments/assets/97a42cdb-b08e-4169-bfc2-6aef1a8d8255" />
Para eliminar por completo la maquina debes seleccionar la casilla que se muestra y luego dale a **Eliminar**


## Con esto concluye la instalacion de Kali Linux desde una maquina virtual 
- Todo fue echo con fines eticos y educativos para el aprendizaje y un entendimiento mas cercano con las maquinas

