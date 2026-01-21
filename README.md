# Lenovo T14 Gen1 Clover EFI

EFI baseada em Clover para ThinkPad T14 Gen1 (Intel).

## Clone
```bash
git clone https://github.com/maxpicelli/Lenovo-T14-Gen1-Clover-EFI.git
```

## Hardware (este setup)
- Modelo: Lenovo ThinkPad T14 Gen1 (Intel)
- CPU: Intel Core i5-10510U (Comet Lake)
- GPU: Intel UHD Graphics 620/630 (iGPU)
- RAM: 16 GB
- Armazenamento: 1 TB NVMe
- Wi-Fi/Bluetooth: Intel AX210 (AirportItlwm + IntelBluetoothFirmware)
- Ethernet: Intel I219-V (IntelMausi)
- Audio: Realtek ALC257 (AppleALC)
- Leitor de cartao: Realtek (RealtekCardReader)
- Thunderbolt: SSDT-TBJHL62 (se aplicavel)

## Bootloader
- Clover (CLOVERX64.efi)
- SMBIOS: MacBookPro16,3 (gere seus proprios seriais)

## ACPI (SSDTs)
- DMAR
- SSDT-BAT0-YOGA
- SSDT-BATXAW
- SSDT-EC-YOT14
- SSDT-Fan-T14
- SSDT-KBD-T14
- SSDT-T14Gen1-USBX
- SSDT-TBJHL62
- SSDT-UIAC
- SSDT-USBX

## Kexts principais
- Lilu, WhateverGreen, AppleALC
- IntelMausi, AirportItlwm, IntelBluetoothFirmware, IntelBTPatcher, BlueToolFixup
- VoodooPS2Controller (Keyboard/Trackpad), VoodooRMI, VoodooSMBus
- USBToolBox + UTBMap, USBWakeFixup
- NVMeFix, RestrictEvents, FeatureUnlock, HibernationFixup, NoTouchID
- ACPIBatteryManager, ACPIPoller, ACPISensors, CPUSensors, FakeSMC, SMCProcessor, SMCLightSensor
- RealtekCardReader + RealtekCardReaderFriend
- YogaSMCAlter

## Observacoes
- Troque SMBIOS/seriais antes de usar.
- Ajuste mapas de USB e SSDTs conforme seu hardware.


