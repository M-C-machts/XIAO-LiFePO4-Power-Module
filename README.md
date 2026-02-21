# XIAO LiFePO4 Module (Charging + 3.3V Regulator)

Small power-management PCB for running an ESP32 (or other 3.3V devices) from a single **LiFePO4** cell.

This board provides:
- **LiFePO4 charging** from ~5V input
- Proper handling of **charge + discharge**
- A **stable 3.3V output**
- **Battery voltage sense** output via a resistor divider (for ADC monitoring)

## Form factor / compatibility

This module matches the **Seeed Studio XIAO** form factor (approx. 21 x 17.5 mm) and is intended to be:
- soldered directly onto a **Seeed Studio XIAO ESP32C3** (castellated-module style), or
- used as a small **daughter board** on a larger PCB.

## Connections

- **Battery**: JST SH connector (LiFePO4 cell)
- **Charge input**: ~5V
- **Output**: regulated 3.3V
- **VBAT_SENSE**: divided battery-voltage output (connect to an ADC pin)

> Pin names / exact pinout depends on the PCB revision. See the schematic/PCB files in this repo.

## Typical use cases

- Battery-powered ESP32 sensor nodes
- Small portable projects using XIAO-sized MCUs
- Projects needing safe LiFePO4 charging + regulated 3.3V

## Notes / safety

- Use only **single-cell LiFePO4** batteries.
- Verify polarity before connecting the battery.
- Charging from ~5V assumes a suitable 5V source (USB, regulated supply, etc.).

## Repo contents

- KiCad project files (schematic + PCB)
- Manufacturing outputs - todo
- BOM / assembly notes - todo

## License

todo