# Default
![](default.gif)

<details><summary>CODE</summary>
<p>

```
GRAB 300
COPY F X
NOTE X = USERNAME
WIPE

LINK 800
GRAB 199

MARK FINDUSER
TEST F = X
FJMP FINDUSER

NOTE FOUND, PROCEED
SEEK 1
COPY F X
DROP

LINK 799
NOTE GRAB USERFILE
GRAB X
COPY 0 X
SEEK 2


MARK READER
ADDI X F X
TEST EOF
FJMP READER

SEEK -9999
SEEK 2


MARK AVGWRITER
NOTE IF X > 75: PUTS 75
TEST X > 75
FJMP ELSE
COPY 75 F
SUBI X 75 X
JUMP AVGWRITER

MARK ELSE
NOTE ELSE: PUTS X
COPY X F
DROP
```
</p>
</details>
