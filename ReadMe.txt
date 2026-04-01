

 




JICO is an app created by Karl Mahlmann intended to promote new music in Just Intonation.
The app is free.  You can support this effort and explore new music in Just Intonation by purchasing the album, "Blest Be the Gluons that Bind".
https://karlmahlmann.bandcamp.com/album/blest-be-the-gluons-that-bind
 
____________________________________________________________________________________________________

Requirements:
This app is compiled with Lazarus/FPC targeting x86_64-win64, so it requires a 64-bit Windows. Specifically:

  - Windows 10 
  - Windows 11 
  - Windows 8.1  (64-bit)
  - Windows 7  (64-bit, with some caveats — some API calls may behave differently)
   it won't run at all 32-bit Windows

The app uses standard Win32/GDI APIs (via LCL), nothing exotic, so compatibility within 64-bit Windows versions should be solid.
____________________________________________________________________________________________________

Installation:
Create a new folder and drop in JICO.exe and any demo files. — for example, C:\Users\YourName\JICO\ or your Desktop.  
That will become JICO's default folder. But do not install it inside C:\Program Files or C:\Program Files (x86), as Windows restricts write access to 
those folders and JICO will be unable to save settings and chord files there.

____________________________________________________________________________________________________

Windows Security Warnings:
JICO.exe is digitally signed with a Microsoft-trusted code signing certificate, which verifies that the program comes from a known publisher and has not been modified since it was signed.

However, you may still see a Windows SmartScreen warning the first time you run it — something like "Windows protected your PC." This is normal and does not mean the program is harmful. SmartScreen assigns a trust rating based partly on how many users have downloaded and run a program. Because JICO is a new release with a small user base, it has not yet accumulated enough download history to be automatically trusted without a prompt.

  To run the program when this warning appears:
  1. Click "More info"
  2. Click "Run anyway"

This prompt will become less common as more users download and run JICO. 
____________________________________________________________________________________________________

Operation Notes:

- MIDI allocates 14 bits for pitch-bend and, per General MIDI Level 1 spec, JICO interprets that numeric range (0 to 16383) as corresponding to +/- 2 semitones.  You should verify that whatever is playing your JICO-generated MIDI file, that it interprets pitch-bend data as spanning +/- 2 semitones. On some DAWs (digital audio workstation) that may be something you set.  

- Once you put a JICO-generated MIDI file into your DAW, you can change the octaves of notes and the pitch bend is unaffected.  But that's just for octaves, The pitch bend data will be invalid (it will be out of tune) if you transpose it in the DAW to some interval other than an octave.  
Of course, you can transpose it any way you want inside of JICO.

-If you define a chord as something other than a simple triad, the notes of that chord are unambiguous, but the program will use its internal logic to select the cells representing those notes. The program attempts to keep the group close together and it takes into consideration preceding chords, but not subsequent chords. So it's possible that you may want something different than what it selects.  One work-around would be to initially have the chord(s) in question sequenced differently. (For example, make the chord(s) in question the first chord.) Then, once the cells are selected, cut and paste the chord(s) into their proper order.  


____________________________________________________________________________________________________

Legal Disclaimer

This software is free. It is provided "as is", without warranty of any kind, express or implied
to the warranties of merchantability, fitness for a particular purpose and noninfringement.
In no event shall the authors or copyright holders be liable for any claim, damages or other
liability, whether in an action of contract, tort or otherwise, arising from, out of or
in connection with the software or the use or other dealings in the software.

____________________________________________________________________________________________________


Contact:
for bug reports, etc.
k18170565@gmail.com

