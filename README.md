# QMK Config for Corne V4.1

This repository contains my custom QMK firmware configuration for the [Corne V4.1](https://github.com/foostan/kbd_firmware/tree/main/keyboards/crkbd/qmk/qmk_firmware) split keyboard. It includes keymaps and layers, specifically designed for my personal use case.

- **QMK Firmware**: To compile and flash your firmware, make sure you have QMK set up. You can follow the [QMK setup guide](https://docs.qmk.fm/#/newbs_getting_started) to get started.
- **Corne V4.1 Keyboard**: This configuration is specifically designed for the Corne V4.1. Ensure your keyboard has the correct hardware.

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/krsntn/qmk-config-corne.git
   cd qmk-config-corne
   ```

2. Install QMK firmware (if not already done):

   ```bash
   python3 -m pip install --user qmk
   ```

3. Set up your QMK environment:

   ```bash
   qmk setup
   ```

4. Compile the firmware for your Corne:

   ```bash
   qmk compile -kb crkbd/rev4_1/standard -km krsntn
   ```

5. Flash the firmware to your Corne:

   1. **Enter Bootloader Mode**:

      - Press and hold the **boot** button, then immediately press the **reset** button to put your Corne into bootloader mode.

   2. **Flash the Firmware**:

      - Once in bootloader mode, simply copy the `.uf2` file to your Corne’s drive to flash the firmware.

## Keymap Overview

### Layers

- **Layer 0**: Default typing layer.
- **Layer 1**: Navigation layer.
- **Layer 2**: Symbols layer.
- **Layer 3**: Numeric keypad layer.
- **Layer 4**: Function keys and media controls layer.
- **Layer 5**: Mouse control layer.

## Configuration

### Keymap File

The main keymap file is located in `config/keymap.c`. You can customize the layout by editing this file.

## Troubleshooting

- **Keymap not flashing?** Make sure you're in the correct bootloader mode for your Corne V4.1.
- **Unexpected behavior?** Check the `keymap.c` file for any syntax errors or conflicts in layer definitions.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- **QMK Firmware**: The foundation for this configuration.
- **Corne Keyboard**: The [Corne V4.1](https://github.com/foostan/kbd_firmware/tree/main/keyboards/crkbd/qmk/qmk_firmware) keyboard design by [foostan](https://github.com/foostan).
- **Community**: Thanks to the QMK and Corne communities for their support and resources.

Feel free to fork, modify, and improve upon this config!
