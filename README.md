# EEPROM-minnet för ATmega328P i C
Implementering av drivrutiner för läsning/skrivning till/från EEPROM-minnet i C.

Filen "ATmega328P device drivers C - EEPROM demo start_code.zip" innehåller startkod för projektet,
vilket innefattar diverse drivrutiner för mikrodator ATmega328P, funktionsbeskrivningar för
drivrutiner till EEPROM-minnet samt instruktioner för vad som ska läggas till för att testa
drivrutinerna i main.c.

Resterande filer utgör samma projekt med färdigskrivna drivrutiner för EEPROM-minnet.
Vid nedtryckning av en tryckknapp ansluten till pin 13 (PORTB5) läses innehållet på adress 1000
i EEPROM-minnet, vilket skrivs ut i terminalen, följt av att samma värde + 1 skrivs tillbaka
till samma adress. Ifall knappen trycks ned kontinuerlig sker läsning/skrivning till/från EEPROM-minnet
en gång i sekunden. 

Testa att dra ut mikrodatorn vid ett visst värde. Koppla seddan in den igen och tryck på knappen.
Notera att det tidigare värdet är bibehållet, då EEPROM-minnet är icke-flyktigt (som programminnet).
Samtidigt går det att skriva och läsa till EEPROM-minnet (likt dataminnet), så EEPROM-minnet utgör
något av en hybrid av programminnet och dataminne.

Se video tutorial här:
https://youtu.be/2XTBsLWfCjc