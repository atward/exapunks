# Default
![](default.gif)

<details><summary></summary>
<p>
XA

```
NOTE SCANNER
LINK 800
LINK 799
GRAB 212

NOTE FOREACH CHANGE
MARK FOREACH
COPY M X

NOTE CHECK IF LAST
TEST X = 1
FJMP SCAN
HALT

MARK SCAN
TEST F = X
FJMP SCAN

NOTE WRITE
SEEK -1
COPY M F
SEEK -9999
JUMP FOREACH
```

XB

```
NOTE INSTRUCTOR
GRAB 300

MARK LOOP
TEST EOF
TJMP END
COPY F M
JUMP LOOP

MARK END
COPY 1 M
```

XC

```
NOTE MV 200 OUTBOX
LINK 800
GRAB 200
LINK 800
```
</p>
</details>
