# Apple Keyboard On Linux

**Fix Mapping for Linux**

Apple Keyboard (A1243) USB Aluminium
Azerty French

### After Boot :

` setxkbmap -variant mac -option apple:badmap fr `

### On Boot :

` nano /etc/default/keyboard `

````
XKBMODEL=""
XKBLAYOUT="fr"
XKBVARIANT="mac"
XKBOPTIONS="apple:badmap"
BACKSPACE="guess"
 ````
\
` update-initramfs -u `
