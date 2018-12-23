# Default
![](default.gif)

<details><summary>CODE</summary>
<p>

```
GRAB 300
LINK 800
COPY 0 #CLRS


MARK LOOP

NOTE ROW
DIVI X 9 #DATA

NOTE COL
MODI X 9 #DATA

NOTE CHAR
COPY F #DATA

NOTE I++
ADDI X 1 X

TEST EOF
FJMP LOOP

WIPE
```
</p>
</details>
