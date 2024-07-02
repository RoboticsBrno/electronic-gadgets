# O co jde?

Hradlo neboli logický člen je základní stavební prvek logických obvodů, který vyčísluje logickou funkci. 
Hradla mají vstupy a typicky jediný výstup. Hodnota na výstupu logického členu je funkcí hodnot vstupních, což znamená, že logická hodnota výstupu je závislá jen na hodnotě vstupu. Naše hradla jsou složena z jednotlivých tranzistorů a rezistoru, které si sami zapájíte tak, aby fungovaly jako logické hradla.

![RoboSvit přední strana](photo/hradla-propag-00.png)

## Značení
Existují dva způsoby značení logických členů (oba definované ANSI/IEEE Std 91-1984 a jeho dodatkem ANSI/IEEE Std 91a-1991). Prvním jsou obdélníkové (čtvercové) značky (IEC, DIN). Druhým způsobem jsou značky složené z křivek (ANSI), které jsou rozšířeny v profesionálních systémech pro návrh logických obvodů. U obou způsobů značení existují v praxi drobné varianty. Negovaný výstup je často označen kolečkem.

![RoboSvit přední strana](photo/logicke_cleny.png)

## Pravdivostní tabulka
Pro ujasnění funkce jednotlivých hradel se používají pravdivostní tabulky, ze kterých je jasně vidět jaké výstupy jsou vytvoří danými vstupy.

### NOT
V programovacích jazycích se obvykle označuje znakem `!`.

| vstup |                 výstup                 |
| :---: | :------------------------------------: |
|   0   | <span style="color:green">**1**</span> |
|   1   | <span style="color:green">**0**</span> |


### AND
V programovacích jazycích se obvykle označuje znakem `&` nebo `&&`.

| vstup-1 | vstup-2 | <span style="color:green">**výstupy**</span> |
| :-----: | :-----: | :------------------------------------------: |
|    0    |    0    | <span style="color:green">**   0   **</span> |
|    0    |    1    | <span style="color:green">**   0   **</span> |
|    1    |    0    | <span style="color:green">**   0   **</span> |
|    1    |    1    | <span style="color:green">**   1   **</span> |

### OR
V programovacích jazycích se obvykle označuje znakem `|` nebo `||`.

| vstup-1 | vstup-2 | <span style="color:green">**výstupy**</span> |
| :-----: | :-----: | :------------------------------------------: |
|    0    |    0    | <span style="color:green">**   0   **</span> |
|    0    |    1    | <span style="color:green">**   1   **</span> |
|    1    |    0    | <span style="color:green">**   1   **</span> |
|    1    |    1    | <span style="color:green">**   1   **</span> |

### NAND
Toto hradlo můžete vytvořit pomocí `AND` jehož výstup znegujete (přivedete na `NOT`).

| vstup-1 | vstup-2 | <span style="color:green">**výstupy**</span> |
| :-----: | :-----: | :------------------------------------------: |
|    0    |    0    | <span style="color:green">**   1   **</span> |
|    0    |    1    | <span style="color:green">**   1   **</span> |
|    1    |    0    | <span style="color:green">**   1   **</span> |
|    1    |    1    | <span style="color:green">**   0   **</span> |

### XOR
V programovacích jazycích se obvykle označuje znakem `^` nebo `^^`.

| vstup-1 | vstup-2 | <span style="color:green">**výstupy**</span> |
| :-----: | :-----: | :------------------------------------------: |
|    0    |    0    | <span style="color:green">**   0   **</span> |
|    0    |    1    | <span style="color:green">**   1   **</span> |
|    1    |    0    | <span style="color:green">**   1   **</span> |
|    1    |    1    | <span style="color:green">**   0   **</span> |

## Terminologie
Někdy se pojmy logický člen a hradlo rozlišují. Pojem hradlo pak označuje fyzickou součástku (např. integrovaný obvod), zatímco pod pojmem logický člen je myšlen prvek realizující logickou funkci.
