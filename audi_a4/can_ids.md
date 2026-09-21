# Audi A4 CAN IDs

Este documento recoge las tramas CAN identificadas experimentalmente en un Audi A4 mediante capturas realizadas desde el conector OBD-II con una Raspberry Pi y un HAT CAN.

Las señales se clasifican como:

✅ Confirmado: validado experimentalmente mediante acciones controladas o comparación con OBD-II.
🟡 Probable / parcial: comportamiento coherente, pero falta validación definitiva.
❓ Desconocido: señal detectada pero función no identificada.

Los bytes se numeran desde B0.

#0x050 — Cinturón del conductor
Byte: B1
Bit: bit4

0 = cinturón desabrochado
1 = cinturón abrochado

Ejemplo observado:

Desabrochado:
B1 = 0x20 = 0010 0000

Abrochado:
B1 = 0x30 = 0011 0000

