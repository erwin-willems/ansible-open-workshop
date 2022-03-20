# Raspberry Pi voorbereiden voor de workshop

## Benodigdheden
Je hebt de volgende onderdelen nodig voor deze workshop:
- Raspberry Pi 3 of 4 (zie Notes)
- Lege Micro SD card (2 GB of meer)
- Voeding voor Raspberry Pi
- Netwerkkabel
- Monitor met HDMI aansluiting (alleen tijdens de installatie)
- HDMI kabel (alleen tijdens de installatie)
- Toetsenbord (alleen tijdens de installatie)

**Note:** Deze workshop werkt op alle Raspberry Pi's die `Raspberry Pi OS Lite (64-bit)` ondersteunen. Zie: https://www.raspberrypi.com/software/operating-systems/#raspberry-pi-os-64-bit voor een lijst van compatible Raspberry Pi's.

## Installatie
We gebruiken tijdens de workshop `Raspberry Pi OS Lite (64 bit)`. 

- Download en installeer de Raspberry Pi Imager, via https://www.raspberrypi.com/software/
- Start de Raspberry Pi Imager
    - Kies `Raspberry Pi OS Lite (64-Bit)` als Operating System
    - Schrijf de image naar je memory card
- Koppel de SD card los en sluit deze weer opnieuw aan op je laptop / computer (zodat de laatste versie van de data zichtbaar wordt)
- Schrijf op de memory card een leeg bestand met de naam: `ssh` naar de boot partitie van de SD card. Dit zorgt er voor dat `ssh` tijdens de eerste start van de Raspberry Pi automatisch gestart wordt.

  **Note:** Let op! dit bestand is hoofdletter gevoellig!

- Plaats de SD card in de Raspberry Pi en start de Pi.

## IP adres achterhalen

Er zijn meedere methodes om het IP adres van je Pi te achterhalen. De meest makkelijke is via een scherm.

### Optie 1

- Voer een ping commando uit naar het adres: `raspberrypi`
- Noteer het IP adres

### Optie 2
- Sluit de Raspberry Pi aan op een scherm
- Sluit de voeding aan en laat de Pi opstarten
- Noteer het IP adres

## Raspberry Pi voorbereiden

Voor de workshop is het belangrijk dat je het volgende hebt gedaan:

- MAC adres genoteerd
- Hostname gewijzigd
- Wachtwoord gewijzigd
