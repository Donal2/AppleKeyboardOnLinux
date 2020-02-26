# Apple Keyboard On Linux

**Fix Mapping for Linux**

Apple Keyboard (A1243) USB Aluminium
Azerty French

### After Booting X :

` setxkbmap -variant mac -option apple:badmap fr `

### Before Boot / No GUI :

` nano /etc/default/keyboard `

````
XKBMODEL=""
XKBLAYOUT="fr"
XKBVARIANT="mac"
XKBOPTIONS="apple:badmap"
BACKSPACE="guess"
 ````
 
` update-initramfs -u `  

### Windows Solution :

https://archive.phocean.net/tools/french-apple-macbook-keyboard-layout-for-windows.html
