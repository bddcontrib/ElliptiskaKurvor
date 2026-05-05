# Elliptiska kurvor

En uppsättning klasser för att hantera elliptiska kurvor, skriven i ren python.
Använder <ins>inte</ins> de coolaste algoritmerna, men fungerar för demonstationssyfte.

## Installation
Klona med:

```
git clone https://github.com/borstelldotdev/ElliptiskaKurvor.git
```

... och importera i en python-fil/använd i konsolen:
```python
from elliptiska_kurvor import Punkt, ElliptiskKurva
```

## Användning
```python
# Importera
>>> from elliptiska_kurvor import Punkt, ElliptiskKurva

# Skapa en elliptisk kurva
>>> e = ElliptiskKurva(a=1, b=1, p=5)
>>> e
Elliptisk kurva `E` i y^2 = x^3 + x + 1 med 9 punkter, projekterad över F5

# Hämta punkter
>>> e.punkter
[Punkt(0, 1), Punkt(0, 4), Punkt(2, 1), Punkt(2, 4), Punkt(3, 1), Punkt(3, 4), Punkt(4, 2), Punkt(4, 3), Punkt(Oändligheten)]

# Hämta en viss punkt
>>> e[0, 1]
Punkt(0, 1)

>>> e.vid(4, 3)
Punkt(4, 3)

>>> e.oändligheten
Punkt(Oändligheten)

# Addera punkter
>>> e[0, 4] + e[4, 2]
Punkt(0, 1)

# Multiplicera en punkt med ett heltal
>>> e[2, 4] * 5
Punkt(2, 1)

```


## Licens
Licenserad under MIT-licensen.
