Installationshinweise aigui Version 1.2
=======================================
Voraussetzungen
---------------
Die Installationsdateien k�nnen in einem beliebigen Verzeichnis gespeichert werden.
F�r die Benutzer ist Lesezugriff ausreichend. F�r den Start unter Windows ist eine 
Netzlaufwerkverbindung zum aigui-Verzeichnis notwendig, da der Start vom aigui-Verzeichnis 
erfolgen muss und der Befehl cd bei Windows f�r UNC-Pfade in der Form "//server/verzeichnis" 
nicht unterstuetzt wird.
Die benutzerspezifischen Konfigurationen werden im Home-Verzeichnis, Unterverzeichnis aigui, 
gespeichert. Bei Windows normalerweise unter C:\Dokumente und Einstellungen\<username>\aigui,
bei UNIX und Linux $HOME\aigui.

Weiterhin ist vom Mathematica das Java-Link Paket JLink erforderlich (JLink.jar, JLinkNativeLibrary.dll).

Installationsdateien
--------------------
aigui.jar              -  Ausf�hrbares Java-Archiv
aigui-changelog.txt    -  �nderungslog
readme_DEU.txt         -  diese Datei
startWinJar.bat        -  Startdatei (siehe Anmerkung)
[conf]                 -  Verzeichnis f�r Konfigurationsdaten
    defaultProperties  -  Standard Properties
	functionOptions    -  Optionen f�r AnalogInsydes Funktionen (z.Z. nicht benutzt)
	functionOptions1   -  Optionen f�r AnalogInsydes Funktionen
	AIStyles.nb        -  Vorlage f�r Notebooks
[JLink-Windows]	       -  Java Link zu Mathematica (*)

(*) nicht erforderlich, wenn JLink bereits installiert ist.
	
Startdatei startWinJar.bat
--------------------------
Die Startdatei enth�lt den Befehl

java -Xmx512m -cp .\aigui.jar;JLink-Windows\JLink.jar aidc.aigui.Gui

Falls JLink bereits in einem anderen Verzeichnis installiert ist, 
muss der Pfad zu JLink.jar gegebenenfalls angepasst werden.

Sonstiges
---------
Fehler, Anmerkungen und W�nsche bitte an volker.boos@imms.de senden.
