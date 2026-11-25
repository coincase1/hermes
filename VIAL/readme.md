# NyxKeys Hermes


The standard Hermes: a 24-key numpad with a dedicated function row (F1–F4), optional 2U Plus, Enter and Zero keys, and a utility column (side depending*).

## Alternative Firmware - Using VIAL

(from Coincase)

The Hermes is shipped with VIA flashed on the board. As mentioned in the main repo, the Hermes is not in VIA's official keyboard list yet (but will be in the future). Hermes users need to go into VIA settings and enabling V2 definitions for now because of this.

Both VIA and VIAL allow you to remap keys. There are some subtle differences but notably approval isn't needed by a maintainer authority for VIAL.

## Flashing the firmware

1. Downlaod ['
1. Download [`hermes_main_v1.0.bin`](hermes_main_v1.0.bin) and install [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases).
2. Open QMK Toolbox and select the `.bin` file.
3. Put the Hermes into bootloader mode (see below). QMK Toolbox should show *"STM32 DFU device connected"*.
4. Click **Flash** and wait for it to finish.
5. Clear the EEPROM after flashing (`Fn` + `.` + `2`) so VIA picks up the default keymap.

In the **Layouts** tab, set **Plus**, **Enter** and **Zero** to match your build: **2U** for a single large key, **Split** for two 1U keys.

## Bootloader

- **Bootmagic reset**: Hold F1 (top-left key) while plugging in the keyboard. This also clears the EEPROM.
- **Reset button**: Briefly press the button on the back of the PCB.
- **Key combo**: Hold `Fn`, then hold `.`, then press `5`.
