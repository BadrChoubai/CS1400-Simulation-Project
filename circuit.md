# Building the Circuit

The simplified Boolean expressions derived from the K-maps were implemented in [Logisim-Evolution](https://github.com/logisim-evolution/logisim-evolution/releases) using AND, OR, and NOT gates.

## Inputs and Outputs

The circuit takes three input pins—`X`, `Y`, and `Z`—and drives seven output signals (`a` through `g`) connected directly to a 7-segment display component.

## Segment Logic

Each segment is driven by the Boolean expression derived from its K-map:

| Segment | Expression  |
| :------ | :---------- |
| a       | X'Y + X'Z   |
| b       | X'Y         |
| c       | X'          |
| d       | Y'Z         |
| e       | X'(Y' + Z') |
| f       | X'(Y + Z)   |
| g       | 1           |

## Notes

- Segment `g` is hardwired to logic `1` — it is always on.
- Segment `c` requires only a single NOT gate.
- Segment `b` requires one AND gate with `X` inverted.

## View the Circuit Images

- [Download decoder.circ](./files/decoder.circ) to run the circuit in Logisim-Evolution.
- [View images of segment logic](./files/segments.png) if you don't want
  to download and run it yourself

