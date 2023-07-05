![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg) ![](../../workflows/test.yaml/badge.svg)

# Barrel shifter

This repository contains the implementation of a barrel shifter for five bit input. The design was implemented through wokwi. The logic diagram of the implementation is shown below.

<p align="center">
<img src=./figures/figure1.png>
</p>
<p align = "center">
    <b>Figure 1:</b> The implementation of the barrel shifter for 5-bit input
</p>

This particular implementation has the ability to shift right or left the input based on the invert bit. The invert bit determines as to whether the input is placed in the higher or lower order bits. For the shift amount two bits are available giving a range between 0 and 3 for the available shifting moves. The result is depicted in the seven segment display where every led depicts the bit position of the final number. For example, if the final result is the number 5, then the leds that are going to light up are the 2 and 0, because the number 5 is represented with the binary 00000101.

# Interface

| Signals | Tiny Tapeout 4 signals |
| :-----: | :--------------------: |
|   In1   |        ui_in[0]        |
|   In2   |        ui_in[1]        |
|   In3   |        ui_in[2]        |
|   In4   |        ui_in[3]        |
|   in5   |        ui_in[4]        |
| shift0  |        ui_in[5]        |
| shift1  |        ui_in[6]        |
| invert  |        ui_in[7]        |
| output  |      uo_out[7:0]       |
