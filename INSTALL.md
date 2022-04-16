# Raspberry Pi voorbereiden voor de workshop

## Benodigdheden
Je hebt de volgende onderdelen nodig voor de workshop:
- Raspberry Pi 3 of 4 (zie Notes)
- Lege Micro SD card (2 GB of meer)
- Voeding voor Raspberry Pi
- Netwerkkabel

Eventueel:
- Een monitor met HDMI aansluiting (alleen tijdens de installatie)
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
  **Note:** Zie ook https://www.raspberrypi.com/documentation/computers/remote-access.html

- Plaats de SD card in de Raspberry Pi en start de Pi.


## IP adres achterhalen

Er zijn meedere methodes om het IP adres van je Pi te achterhalen. De meest makkelijke is via het ping commando.

### Optie 1

- Voer een ping commando uit naar het adres: `raspberrypi`
- Noteer het IP adres

### Optie 2
- Sluit de Raspberry Pi aan op een scherm
- Sluit de voeding aan en laat de Pi opstarten
- Log in als gebruiker `pi`
- Voer uit: `ip addr`
- Noteer het IP adres

## Raspberry Pi voorbereiden

Voor de workshop is het belangrijk dat je het volgende hebt gedaan:

- Wachtwoord gewijzigd
- Hostname gewijzigd

### Wachtwoord wijzigen

Het wachtwoord wijzigen kan met `raspi-config`. 

- Log in op je Pi (via SSH of via een aangesloten scherm) met de gebruiker `pi`
- Voer uit: `sudo raspi-config`
- Kies `S3 Password`
- Vul een nieuw wachtwoord in

### Hostname wijzigen

Om tijdens de workshop je Pi terug te vinden in het netwerk is het handig om de hostname te wijzigen. Dit gaat het makkelijkst met `raspi-config`.

- Kies in het menu `1 System Options`
- Kies `S4 Hostname`
- Geef je Pi een eigen hostname
- Reboot de Pi

Controlleer of je via de hostname en met het nieuwe wachtwoord in kunt loggen op je Pi
