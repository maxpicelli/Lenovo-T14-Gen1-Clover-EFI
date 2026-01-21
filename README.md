# Lenovo T14 Gen1 Clover EFI

EFI baseada em Clover para ThinkPad T14 Gen1 (Intel).

## Hardware (este setup)
- Modelo: Lenovo ThinkPad T14 Gen1 (Intel)
- CPU: Intel 10th Gen (Comet Lake-U) [preencher modelo exato]
- GPU: Intel UHD (iGPU)
- RAM: [preencher]
- Armazenamento: [preencher]
- Wi-Fi/Bluetooth: Intel (AirportItlwm + IntelBluetoothFirmware)
- Ethernet: Intel (IntelMausi)
- Audio: AppleALC
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

## Status
- macOS testado: [preencher]
- Funciona: [preencher]
- Nao testado: [preencher]
