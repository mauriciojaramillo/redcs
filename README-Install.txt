REDCS - RED COMUNIDAD SOLIDARIA / 2020
Connectividad.net / Colombia


Installation instructions for Twilio Hackathon demo.


PREREQUISITES
-------------
1- Windows Server 2008 or Windows 10 (or later).

2- SQL-Server 2008 (or later), Express edition (or higher) and SQL-Server Management console. TCP/IP protocol enabled.

3- Node.JS v11.8.0. and NPM.

4- TCP ports available: 80, 443 and 3001.



+++

INSTALL
-------
1- Download the 2 files (RedCS-AppCode.zip and RedCS-DataBases.zip) and save on your local disk.


2- Create the following folders on your local disk:
   C:\App                    (root folder)
   C:\App\redcs              (app folder)
   C:\App\redcs-archivos     (working files folder)
   C:\App\redcs-db           (databases folder)


3- Extract the files from "RedCS-AppCode.zip" in the folder "C:\App\redcs" (11 folders and 2 files contained at root).


4- Extract the files from "RedCS-DataBases.zip" in the folder "C:\App\redcs-db" (4 files contained).


5- Using "SQL-Server Management console" attach the 2 databases contained in "C:\App\redcs-db" folder; select the files "uaw_v4_datos.mdf" and "uaw_v4_metadatos.mdf" respectively for this task. Let the sugested names "uaw_v4_sos01_datos" and "uaw_v4_sos01_metadatos" for databases.

Note: if you are using "SQL-Server Express Edition" we strongly recommend to turn off "Auto Close" option on 2 DBs for optimal performance.


6- Using "SQL-Server Management console" create a new "SQL-Server user" with name "sos01" and password "NoHayClave" (you may change this later for stronger security) and set default languaje to "Spanish"; grant privileges "db_owner" and "public" to the recently created user over the 2 databases.


7- Open "Command line" or "Power shell" console in the folder "C:\App\redcs" and run the following command to install required Node.js modules:

    npm install


8- Open "Command line" or "Power shell" console in the folder "C:\App\redcs" and run the following command to start the application:

    node bin/www


9- Wait a few seconds and the following message must be shown on the screen; now, You are ready to use the App:

+---------------------------------------------------------------+
|                                                               |
|          YA PUEDE INICIAR SU TRABAJO EN EL SISTEMA            |
|                                                               |
+---------------------------------------------------------------+


10- Open your browser an visit "https://your_ip_address"; You will be redirected to "https://your_ip_address/redcs/" to begin using the App.


11- Open the file "README-Use.txt" (download from the repository) to view some instructions for use; We are using a SandBoxed account and need a little more steps to be ready.


+++

Created: 2020/04/30
Mauricio Jaramillo
Alfonso Ortega


Modified:

