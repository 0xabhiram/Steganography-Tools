# Steganography-Tools

What is Steganography?
Steganography has evolved from the Greek word “Steganos” meaning hidden or covered. Steganography is the art of hiding a secret message into an ordinary object. The secret message and ordinary objects can be an image, text, audio, files etc. A user can hide the secret in an ordinary looking object using some tools and techniques and the receiver can then use the similar technique to get the secret back.

<h1>Top 10 tools to perform Steganography</h1>
<h4>1. Steghide:</h4>
Steghide is a steganography program that hides data in various kinds of image and audio files , only supports these file formats : JPEG, BMP, WAV and AU. but it’s also useful for extracting embedded and encrypted data from other files.<br>
It can be installed with apt however the <a href="https://github.com/StefanoDeVuono/steghide">Source </a>can be found on github.



## Useful commands:

```
steghide extract -sf file
```

<h4>2.Foremost</h4>
Foremost is a program that recovers files based on their headers , footers and internal data structures , I find it useful when dealing with png images.

## Useful commands:
```
foremost -i file
```
<h4>3.Stegsolve:</h4>
Sometimes there is a message or a text hidden in the image itself and in order to view it you need to apply some color filters or play with the color levels. You can do it with GIMP or Photoshop or any other image editing software but stegsolve made it easier. it’s a small java tool that applies many color filters on images. Personally i find it very useful.Personally i find it very useful.
You can get it from <a href="https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve">github</a>

<h4>4.Exiv2</h4>
A tool similar to exiftool.<br>
It can be installed with apt however the <a href="https://github.com/Exiv2/exiv2">source</a> can be found on github.
<a href="https://exiv2.org/">Official website</a>

## Useful commands:
```
exiv2 file
```
<h4>5.Binwalk</h4>
Binwalk is a tool for searching binary files like images and audio files for embedded files and data.
It can be installed with apt however the source can be found on <a href="https://github.com/ReFirmLabs/binwalk">github.</a>

## Useful commands:
```
binwalk -e file
```


<h4>6.Zsteg</h3>
zsteg is a tool that can detect hidden data in png and bmp files.
to install it : <b>gem install zsteg</b> ,The source can be found on <a href="https://github.com/zed-0xff/zsteg">github</a>

## Useful commands:
```
zsteg -a file
zsteg -E file
```
<h4>7.Wavsteg</h4>
WavSteg is a python3 tool that can hide data and files in wav files and can also extract data from wav files.
You can get it from <a href="https://github.com/ragibson/Steganography#WavSteg">github</a>

## Useful commands:
```
python3 WavSteg.py -r -s soundfile -o outputfile
```

<h4>8.Sonic</h4> 
Sonic visualizer is a tool for viewing and analyzing the contents of audio files, however it can be helpful when dealing with audio steganography. You can reveal hidden shapes in audio files.
<a href="https://www.sonicvisualiser.org/">Offical Website</a>

## Useful commands:
```
sonic-visualiser <file_name>
```
<h4>9.Fcrackzip</h4>
Sometimes the extracted data is a password protected zip , this tool bruteforces zip archives.
It can be installed with apt however the source can be found on <a href="https://github.com/hyc/fcrackzip">github.</a>

## Useful commands:

```
fcrackzip -u -D -p wordlist.txt file.zip 
```

## Challenges
Some platforms to solve stego challenges <a href="https://www.hackthebox.com/">HackTheBox </a> <a href="https://www.root-me.org/">rootme</a>  <a href="https://ringzer0ctf.com/challenges">RingerZeroCTF</a>



