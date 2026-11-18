# ASUS A8N32-SLI Deluxe — BIOS 1409 O.C. Profile Mod

Modified AMIBIOS8 firmware for the **ASUS A8N32-SLI Deluxe**, based on ASUS BIOS **1409**.

Image: `A8SDA204.ROM`, 1 MiB.

<img width="2200" height="1237" alt="grafik" src="https://github.com/user-attachments/assets/d6c90a54-1154-4fcc-8394-6006705f16af" />


## Features

- Two BIOS setup profiles stored in flash NVRAM.
- Save/load menu: **Exit → ASUS O.C. Profile**. Apply loaded settings with **Save & Exit**.
- Standard **Load Setup Defaults** remains available.

The main module uses AMI LH5 compression. Module and main BIOS checksums are valid for ASUS AFUDOS 1.19.

## Validation

Hardware testing confirmed correct operation with all BIOS settings and successful DOS flashing. Both profiles remain persistent after mains power removal and a CMOS reset.

## Flashing

Back up the existing chip contents before flashing.

Copy the included `AFUDOS.EXE` (ASUS AFUDOS 1.19) and `A8SDA204.ROM` to the DOS drive, then run:

```text
AFUDOS /iA8SDA204.ROM
```

Use only on the specified board; recovery from a failed flash may require an external programmer.

## NVRAM

The supplied image contains the initial backup NVRAM with empty profile slots. Existing profiles on the board may be overwritten depending on the flashing method.

This is an unofficial modification; original firmware and AFUDOS rights remain with their respective owners.
