# Projekt Smarthome 1

En opgave der handler om at udvikle et IOT-smarthome styresystem til min makkers hjem i Java.

## Problem domain

Interview med Niels:

1. Lys.  
a) Tænd og sluk af lys ved hjælp af bevægelsessensor.

2. Kaffemaskinen.  
a) Tænd/sluk.

3. Varme.  
a) Termostat regulering af varme, så der ikke bliver for koldt.

4. El.  
a) Tænd/sluk af alle stand by devices (dimser) som f.eks. Routor, switch, TV, TV box, Microbølgeovn, DeskTop og Monitor.   
b) Constraint: Må IKKE slukke for Køleskab/Fryser.

5. Vindue.   
a) Åbner vindue; slukker for varmen / Lukker vindue; tænder for varmen igen.

## Use cases

Lyset skal tænde når Niels kommer hjem og er inde i rummet og slukke når han ikke er i rummet.   
Kaffemaskinen tænder automatisk på et bestemt tidspunkt og laver kaffe til ham.   
Varme termostaten regulærer varmen så rummet ikke bliver for koldt.   
Når hans devices/enheder går på standby og ikke bliver brugt, bliver der slukket for strømmet til de devices/enheder.   
Når vinduet bliver åbnet, slukker varmen og når man lukker det bliver varmen tændt igen, så man sparer på varmen.

## Design your classes

Super klasse: Lys   
Sub klasse: Tænd_og_sluk_bevægelse

Super klasse: Kaffemaskine   
Sub klasse: Tænd_og_sluk_tid

Super klasse: Varme   
Sub klasse: Termostatregulator

Super klasse: El
Sub klasse: Tænd_og_sluk_standby_devices

Super klasse: Vindue
Sub klasse: Tænd_og_sluk_vindue
