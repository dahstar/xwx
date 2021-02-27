for Simple Steganography can use strings exiftool and like that 
on https://ctflearn.com/challenge/894 use steghide
first get password from image 
strings -a Minions1.jpeg | head -5
JFIF
0Photoshop 3.0
8BIM
myadmin
!1#%)+...
then
use command
steghide --extract -sf Minions1.jpeg
Enter passphrase: myadmin(steghide need password)
wrote extracted data to "raw.txt".
because raw.txt is base64 number so use
cat raws.tx |base 64 -d 
CTFlearn{this_is_fun}
