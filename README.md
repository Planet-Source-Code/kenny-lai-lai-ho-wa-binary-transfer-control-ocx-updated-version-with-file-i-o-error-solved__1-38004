<div align="center">

## \[Binary Transfer Control OCX Updated version with File I/O Error solved\] Extremely fast


</div>

### Description

<p>[Binary Transfer Control OCX] Extremely fast, almost NO MEMORY USE, reliable,

as easy to use as an ordinary Winsock control. Every network programmer must

use, and every one must see!</p>

<p>This is an OCX version of a completely new binary transfer engine. <b>It

sends a 244MB file in 71 seconds and I can still work on another VB IDE without

effort!</b> The sender control read-and-send one chunk only for each time, using

the same array of a chunk size (Optimum is 4096 bytes). Once the receiver

control receive the bytes, it builds up the file immediately. It's hard-drive

and CPU intensive, but using almost no memory! (You can monitor the memory usage

while sending file.)</p>
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Kenny Lai, Lai Ho Wa](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/kenny-lai-lai-ho-wa.md)
**Level**          |Advanced
**User Rating**    |4.7 (93 globes from 20 users)
**Compatibility**  |VB 6\.0
**Category**       |[Internet/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-html__1-34.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/kenny-lai-lai-ho-wa-binary-transfer-control-ocx-updated-version-with-file-i-o-error-solved__1-38004/archive/master.zip)





### Source Code

<p>[Binary Transfer Control OCX] Extremely fast, almost NO MEMORY USE, reliable,
as easy to use as an ordinary Winsock control. Every network programmer must
use, and every one must see!</p>
<p>This is an OCX version of a completely new binary transfer engine. <b>It
sends a 244MB file in 71 seconds and I can still work on another VB IDE without
effort!</b> The sender control read-and-send one chunk only for each time, using
the same array of a chunk size (Optimum is 4096 bytes). Once the receiver
control receive the bytes, it builds up the file immediately. It's hard-drive
and CPU intensive, but using almost no memory! (You can monitor the memory usage
while sending file.)</p>
<hr>
<p>Last time I upload a sample to upload file using multiple winsocks and arrays
and collection of bytes. The speed is about 1600KBps. But many people complain
about the memory usage that store all the bytes of a large file.&nbsp;</p>
<p><b>This time I have changed my mind. I use chunks only, with DoEvents in all
FileIO and sending work. The sender read a chunk from file and send it
immediately, while the reader build up the bytes to the target file once it get
the bytes.</b></p>
<p><b>The speed is awesome. The top speed while sending the Office 2000 Disc 1
zip file(244 MB) is &gt;4200KBps (32.8125Mbps). This meet the industrial
standard (The maximum capacity of a small-business server is about 45Mbps, but
the server administrator will definitely not allow one client to draw all the
bandwidth.</b></p>
<p>The zip file contain two part. The files in the top directory is a
User-Control test that I used to build the control for debug. The OCXs and Test
project is inside the OCX Test directory. There's an OCX included, and the BinaryTransferOCXTest.exe
use the reference of the BinaryTransferControl.ocx.</p>
<p>Using standalone OCX has an advantage that it uses multithread. The entire
program will not be affected while the control is busing sending files. <b>(REMARK:
If you test the program on local-to-local with very large, &gt;300MB files, the
program itself may be affected as it draw all the CPU and HardDrive power to
transfer and receive bytes. But in real situation, the CPU and HardDrive effort
is directly depend on the network speed. That mean the engine draw and send and
build up bytes ONLY when the last bytes is sent or received.)</b></p>
<p>The demonstration program in the OCX Test directory(BinaryTransferOCXTest.vbp)
is well written and run smoothly. (As the screenshot show, it sends the
Office2000 Disc 1 in ZIP effortlessly.) <b>PLEASE FOLLOW THE ORDER OF CALLING
METHOD STRICTLY ACCORDING TO THE DEMONSTRATION, AS THE METHODS AND EVENTS ARE
HIGHLY INTERDEPENDENT!</b></p>
<p>Finally, please vote my work and give any comments, and critics.</p>
<p>Thank you for reading this long long article.</p>
<p>Kenny Lai</p>
<p><a href="http://pcseries.sourceforge.net/pscode/BinaryTransferControl.zip">http://pcseries.sourceforge.net/pscode/BinaryTransferControl.zip</a></p>

