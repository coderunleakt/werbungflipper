##Werbung mit Flipper##
#Berufliches Gymnasium Technik##
────────────────────────────────────
Tom Holland
BGT221




#Erklärungen#
BadUsb
“hackt” einen Computer, es öffnet sich ein “Ausführen” fenster, öffnet Eingabeaufforderung, erstellt editor datei und schreibt text + TBZ Logo
! NUR WINDOWS FUNKTIONIERT
Evil-Portal
erstellt ein Wlan Names “Tbz_guest”, dort kann man sich im TBZ Gast Wlan anmelden. Es gibt kein wirkliches WLAN, die Anmeldedaten werden auf dem Flipper gezeigt. 
!!! Erinnert die Menschen, keine Echten Daten abzugeben
#Backups!#
Erstellt vor jedem Versuch, wo ihr etwas ändert, ein Backup - es kam oft genug vor, wo am Ende sehr aufwendige Projekte wie die Schranke neu gemacht werden mussten.
Links BadUSB:


#Links Evil-Portal#
2.0 evil-portal github: https://github.com/bigbrodude6119/flipper-zero-evil-portal/tree/main?tab=readme-ov-file 
2.1 Grundlegendes Erklärungsvideo: https://www.youtube.com/watch?v=WPT7qeySf6g&t=337s
2.2 Assets zum Hinzufügen: https://github.com/bigbrodude6119/flipper-zero-evil-portal/releases
#Firmware:#
2.3https://github.com/DarkFlippers/unleashed-firmware/blob/dev/documentation/HowToInstall.md - how to update Firmware
2.4https://github.com/xMasterX/all-the-plugins#extra-pack - Erklärung wo was drinne ist
2.5https://github.com/DarkFlippers/unleashed-firmware/releases - unrealised auflistung 
#Firmware#
-> sobald updates über QFlipper gemacht werden, setzt sich sich automatisch auf die neuste ORIGINALE Version zurück, hierdurch können Projekte nicht mehr funktionieren
Es git bestimmte Arten, welche alle Unterschiedliche Zusatzmodule haben: (Link 2.4)
vore MUSS flipper-z kommen |  f7 (=hardware version) überall gleich
unlshd-078 = Firmware version | je nachdem, welche Verison ihr haben wollt
ohne buchstaben: base apps
c: -
e: base apps + extra apps
r: base apps + extra + rgb = NUR MODDED, STAND 04.12.2024 NICHT FÜR DEN SCHULFLIPPER


base apps: vorinstalliert vom flipper
extra apps: zusatzmodule 


#How to BadUSB#
siehe firmware - base apps reicht hierfür // oder offizielle firmware update
siehe Dateien Ordner für speziell TBZ Logo


#How to Evil-Portal#


1. Dev Board an PC anschließen 
2. Download wifi_dev_board.zip (Link 2.2)








3. Flipperlab öffnen 
1. Chrome / Edge am besten 
   1. Als Administrator
   2. seriellen port zulassen
https://support.google.com/chrome/answer/12576972?hl=de 
b. click connect -> esp32 (flipper wifi board) auswählen
c. füge jeweilige Dateien aus wifi_dev_board.zip passend hinzu:
   * 1000 - EvilPortal.ino.bootloader.bin
   * 8000 - EvilPortal.ino.partitions.bin
   * e000 - boot_app0.bin
   * 10000 - EvilPortal.ino.bin


d. offentlich done - board entfernen, braucht ihr erstmal nicht mehr


4. Flipper an PC anschließen
   1. QFlipper oder Flipperlab öffnen
   2. Flipper anschließen


   1. download: unleashed-evil_portal.fap.zip
   2. entpacken und speichert wo ihr wollt
Ordnerstruktur anlegen: // auf dem Flipper
apps/
  GPIO/
    hier kommt der Download hin: evil:portal.fap
apps_data/
  evil_portal/
    //siehe nächster schritt








5. lade evil_portal_sd_folder.zip herunter
   1. cd evil_portal/
   2. öffne ap.config.text
   1. der text der dort steht ist der Name von dem WLAN Hotsopt - anpassbar
   3. ziehe ap.config.txt in den ordner evil_portal


   1. cd evil_portal/
   2. öffne index.html
   1. das ist die Website, welche beim Verbinden angezeigt wird - anpassbar mit html und css (müssen in einer klasse sein, kein link dazwischen)
   3. ziehe index.html in den ordner evil_portal


6. ziehe alles ab, gehe über den Flipper in apps/GPIO und öffne evil-portal, 
start = hotspot starten
-> im feld werden die sachen angezeigt, welche eingeben werden, nachdem auf anmelden geklickt wurde
stop = stoppen
-> alles andere ist tiefergehend und für Einführung in Werbung unteresesant, kann man Sachen wie trolls und wirklich attacken machen


=> Wenn Firmware zu alt, nicht einfach die neue installieren, es ist der Falsche Buchstabe installiert
