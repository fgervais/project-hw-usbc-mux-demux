# USB-C mux/demux

![Overview](assets/img/overview.jpg)

## Use-cases

Basically used to mux or demux usb 2.0 data bus with USB-PD up to and including
revision 3.1 at 48V.

Here's an illustration highlighting a couple use-cases:

![Use-Cases](assets/img/use-cases.jpg)

## Switching converter analysis

![Overview](assets/img/sw_node_overview.jpg)

50 ohms series termination at the SW node.

![Closeup](assets/img/sw_node_closeup.jpg)

### Switch node

| Input Voltage | Waveform | Rising edge |
|---------------|----------|-------------|
| 10V           | ![Waveform](assets/img/sw_node_10V_400mA/DS2_QuickPrint78.png) | ![Rising](assets/img/sw_node_10V_400mA/DS2_QuickPrint79.png) |
| 20V           | ![Waveform](assets/img/sw_node_20V_400mA/DS2_QuickPrint81.png) | ![Rising](assets/img/sw_node_20V_400mA/DS2_QuickPrint80.png) |
| 48V           | ![Waveform](assets/img/sw_node_48V_400mA/DS2_QuickPrint86.png) | ![Rising](assets/img/sw_node_48V_400mA/DS2_QuickPrint87.png) |
