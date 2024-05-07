# Discovering Resistor-Transistor Logic (Building AND gates the wrong way)

This video explores a variation of the gate from the [Part III](../and-gates-transistors/). The resulting gate appears to work but inverts
the output, resulting in a NAND gate. By using an additional transistor as a NOT gate, the result can be fixed into a working AND gate.


Check the video first:

<iframe width="560" height="315" src="https://www.youtube.com/embed/hAYQe-wHV3I?si=sa5FE-8SBPUGFOkN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Schematics

* [Download full schematic](schematic.png)
* [Download KiCAD schematic](../../kicad/and-gates-p4/and-gates-p4.kicad_sch)

## What materials you need

If you want to rebuild this, check the video to see how many gates you want to build (the video starts with one, then goes to three), and adjust materials accordingly

* Input circuitry (pair of inputs):
  * 2 × SPDT switches. (A DPDT one will also work)
  * 2 × LED as indicator (optional)
  * 2 × LED protection resistor, if you use indicator LEDs (I used a 1KΩ because my green LEDs are very bright)
* Per gate (depending how many you want to build):
  * 3 × PN2222A transistors
  * 2 × 10KΩ resistors
  * 1 × 1KΩ resistor
* Output
  * 1 × LED. Any color will work; but if you built the composed three gates try both with a red and a blue one.
  * 1 protection resistor for LED (330Ω is a reasonable amount, adjust according to preference)

### Can I use a different transistor?

See [discussion in Part III](../and-gates-transistors/README.md#can-i-use-a-different-transistor).

## Data sheets

* [PN2222A](https://users.ece.utexas.edu/~valvano/Datasheets/PN2222-D.pdf) NPN Bipolar Junction Transistor.