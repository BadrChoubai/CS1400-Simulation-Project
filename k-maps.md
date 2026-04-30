# Karnaugh Maps

A Karnaugh map is a diagram used to simplify Boolean algebra expressions [^1]. This project required constructing a K-map for each segment of the output display.

## Segment A

| **Segment A** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `0` |
| **X'Y**       | `1` | `1` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
X'Y + X'Z
$

## Segment B

| **Segment B** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `0` | `0` |
| **X'Y**       | `1` | `1` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
X'Y
$

## Segment C

| **Segment C** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `1` |
| **X'Y**       | `1` | `1` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
X'
$

## Segment D

| **Segment D** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `0` |
| **X'Y**       | `0` | `0` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
Y'Z
$

## Segment E

| **Segment E** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `1` |
| **X'Y**       | `0` | `1` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
X'(Y' + Z')
$

## Segment F

| **Segment F** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `0` |
| **X'Y**       | `1` | `1` |
| **XY**        | `0` | `0` |
| **XY'**       | `0` | `0` |

### Boolean Expression

$
X'(Y + Z)
$

## Segment G

| **Segment G** | Z   | Z'  |
| :------------ | :-- | :-- |
| **X'Y'**      | `1` | `1` |
| **X'Y**       | `1` | `1` |
| **XY**        | `1` | `1` |
| **XY'**       | `1` | `1` |

### Boolean Expression

$
G = 1
$

---

### References

[^1]: https://en.wikipedia.org/wiki/Karnaugh_map
