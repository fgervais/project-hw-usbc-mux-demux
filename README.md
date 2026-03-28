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

### Output (5V)

![Overview](assets/img/output.jpg)

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_10V/DS2_QuickPrint103.png) | ![Waveform](assets/img/output_10V/DS2_QuickPrint104.png) | ![Waveform](assets/img/output_10V/DS2_QuickPrint105.png) | ![Waveform](assets/img/output_10V/DS2_QuickPrint106.png) |
| 20V           | ![Waveform](assets/img/output_20V/DS2_QuickPrint107.png) | ![Waveform](assets/img/output_20V/DS2_QuickPrint108.png) | ![Waveform](assets/img/output_20V/DS2_QuickPrint109.png) | ![Waveform](assets/img/output_20V/DS2_QuickPrint110.png) |
| 48V           | ![Waveform](assets/img/output_48V/DS2_QuickPrint111.png) | ![Waveform](assets/img/output_48V/DS2_QuickPrint112.png) | ![Waveform](assets/img/output_48V/DS2_QuickPrint113.png) | ![Waveform](assets/img/output_48V/DS2_QuickPrint114.png) |

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_10V_noise/DS2_QuickPrint115.png) | ![Waveform](assets/img/output_10V_noise/DS2_QuickPrint116.png) | ![Waveform](assets/img/output_10V_noise/DS2_QuickPrint117.png) | ![Waveform](assets/img/output_10V_noise/DS2_QuickPrint118.png) |
| 20V           | ![Waveform](assets/img/output_20V_noise/DS2_QuickPrint121.png) | ![Waveform](assets/img/output_20V_noise/DS2_QuickPrint122.png) | ![Waveform](assets/img/output_20V_noise/DS2_QuickPrint123.png) | ![Waveform](assets/img/output_20V_noise/DS2_QuickPrint124.png) |
| 48V           | ![Waveform](assets/img/output_48V_noise/DS2_QuickPrint125.png) | ![Waveform](assets/img/output_48V_noise/DS2_QuickPrint126.png) | ![Waveform](assets/img/output_48V_noise/DS2_QuickPrint127.png) | ![Waveform](assets/img/output_48V_noise/DS2_QuickPrint128.png) |

### Noise

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | 17.60 mV (0.35%) | 19.80 mV (0.40%) | 13.00 mV (0.26%) | 12.40 mV (0.25%) |
| 20V           | 13.40 mV (0.27%) | 14.80 mV (0.30%) | 15.20 mV (0.30%) | 15.40 mV (0.31%) |
| 48V           | 15.00 mV (0.30%) | 17.60 mV (0.35%) | 28.20 mV (0.56%) | 19.60 mV (0.39%) |
