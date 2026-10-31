# Steam Controller 2 - OpenPuck 500 Hz firmware

Builds the [OpenPuck](https://github.com/safijari/openpuck) firmware with `POLL_US_DEFAULT` set to 2000 us (500 Hz)
instead of the stock 4000 us (250 Hz). The GitHub Actions workflow in `.github/workflows/build-500hz.yml` applies the
change, builds with the repo's own `make uf2`, verifies the UF2 and saves it to `firmware/OpenPuck-500Hz.uf2`.

Flash it from the Firmware update tab at https://safijari.github.io/openpuck/ or drag it onto the board in DFU mode.
