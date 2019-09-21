# GP proto CNC60100

Passi per configurare il software UCCNC sul computer:

1. Attiva .NET framework versioni 3.5 and 4.7 in Windows, dal menu **Attiva o disattiva funzionalità di Windows**.
1. Connetti la macchina
1. Installa *UCCNC*, usando la posizione predefinita `C:\UCCNC`. **Non avviare UCCNC**
1. Copia la cartella Profiles nella cartella di *UCCNC* 
1. Copia il file di licenza nella cartella di *UCCNC*
1. Tasto destro sull'icona sul desktop -> Proprietà
1. Cambia la stringa Destinazione in `C:\UCCNC\UCCNC.exe /p GP010-1000`, così che apra il profilo della CNC60100 di default. 
1. Apri UCCNC dall'icona sul desktop

## CAM

Fusion360 offre funzionalità di CAM gratuitamente per applicazioni senza fini di lucro. È necessario scaricare un postprocessor per UCCNC. Il postprocessor è scaricabile all'indirizzo: https://cam.autodesk.com/hsmposts?p=uccnc
Per installare il postprocessor è sufficiente scaricare il file dal sito di autodesk e copiarlo nella cartella dei postprocessor di Fusion360

#### Workflow base per Fusion360
Una volta disegnato il modello 3D del pezzo da lavorare, e dopo averlo aperto in Fusion360, è possibile passare alla scheda "Manufacture".  
Un'indicazione generale dei passaggi necessari per ottenere un programma utilizzabile con UCCNC è la seguente:

1. Creare un setup, inserendo l'orientamento degli assi, le dimensioni dello stock ed eventualmente i punti di fissaggio.
1. Inserire le lavorazioni necessarie
1. Generare i percorsi
1. A questo punto è buona pratica controllare attentamente la simulazione prodotta da Fusion, per accertarsi che non ci siano errori di programmazione
1. Dal menu Actions, selezionare l'opzione Post process, indicare di voler utilizzare il postprocessor di UCCNC e salvare il file
