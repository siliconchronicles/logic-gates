# Transistors are switches? (Building AND gates the wrong way)

This video explores a simple gate based on the idea of using transistor as switches in a similar way to our gate in [Part I](../and-gates-intro/). The resulting gates work in simple cases. However they degrade the signal so they are not composable unless you re-amplify them. They need you to be especially careful about the resistor values.

Check the video first:

<iframe width="560" height="315" src="https://www.youtube.com/embed/7ssqE-jimCQ?si=cZcZ4X-MRVE0DnE7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Schematics

* [Download full schematic](schematic.png)
* [Download KiCAD schematic](/kicad/and-gates-p3/and-gates-p3.kicad_sch)

## What materials you need

If you want to rebuild this, check the video to see how many gates you want to build (the video starts with one, then goes to three), and adjust materials accordingly

* Input circuitry (pair of inputs):
  * 2 × SPDT switches. (A DPDT one will also work)
  * 2 × LED as indicator (optional)
  * 2 × LED protection resistor, if you use indicator LEDs (I used a 1KΩ because my green LEDs are very bright)
* Per gate (depending how many you want to build):
  * 2 × PN2222A transistors
  * 2 × 10KΩ resistors
  * 1 × 1KΩ resistor
* Output
  * 1 × LED. Any color will work; but if you built the composed three gates try both with a red and a blue one.
  * 1 protection resistor for LED (330Ω is a reasonable amount, adjust according to preference)

### Can I use a different transistor?

The circuit I have there should work with most NPN bipolar junction
transistors, as long as they can handle the voltage used by your
circuit. Other popular ones should be the BC547 or a 2N3904.

Some variants like the P2N2222A or 2N2222A will work the same.

If you choose a different one, check the data sheet for your exact
model number to see which pin
corresponds to base, collector and emitter. Even close variants can
have variations.

## Data sheets

* [PN2222A](https://users.ece.utexas.edu/~valvano/Datasheets/PN2222-D.pdf) NPN Bipolar Junction Transistor.

