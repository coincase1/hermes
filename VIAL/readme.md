# NyxKeys Hermes - Vial Firmware

(from Coincase)

The standard Hermes: a 24-key numpad with a dedicated function row (F1–F4), optional 2U Plus, Enter and Zero keys, and a utility column (side depending on orthodox/southpaw*).

The Hermes is shipped with VIA flashed on the board. As mentioned in the main repo, the Hermes is not in VIA's official keyboard list yet (but will be in the future). Hermes users need to go into VIA settings and enabling V2 definitions for now because of this.

Both VIA and VIAL allow you to remap keys. There are some subtle differences but notably approval isn't needed by a maintainer authority for VIAL.

## Flashing the firmware

1. Download ['hermes_sp_vial.bin'](hermes_sp_vial.bin) and install [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases).
2. Hold down the "reset" switch on the back of the hermes PCB while connecting it to your PC.
3. Open QMK Toolbox. There should be one STM32 device listed in yellow or an alternative color, indicating that it is ready to be flashed.
4. Select the '.bin' file from #1 with the Local File "Open" button.
5. Click **Flash** and wait for it to flash.
6. Go to ['vial.rocks'](vial.rocks) to configure your Hermes to your liking. Any changes there should be saved to your keyboard. Alternatively there is an offline vial utility that can be downloaded for configuring elsewhere.

In the **Layouts** tab, set **Plus**, **Enter** and **Zero** to match your build: **2U** for a single large key, **Split** for two 1U keys.

## Bootloader

The bootloader shortcuts are still available in VIAL. You should see these on Layer 2.

## Special Thanks

Thank you to Shiva1796/Nyxkeys for sharing their original QMK/VIA code. Most of it carries over to VIAL seamlessly.
