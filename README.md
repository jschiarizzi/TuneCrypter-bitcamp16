**Inspiration**
Victoria's dream job is to combine my interests of CS, Criminal Justice, and forensics, and work in digital forensics one day, so I thought I'd take a crack at making my own steganography-like application!

What it does
This application has two layers of encryption: it is designed to take whatever text input you give it, hash it with an undisclosed algorithm, and conceal it within a music (.wav) file. On the other end, the decrypt takes the music file and the two keys (music and algorithm) and reveals the original message.

How I built it
I used the NAudio open source library to process the sound files, and Visual Studio to build the application and GUI in C#.

Challenges I ran into
NAudio and .wav formats in general were really difficult to understand and find documentation on, so a lot was trial and error to test my theories of how best to conceal a message without disrupting the original sound file too much.

The implementation of encoding/decoding the music (and what exactly to /do/ with it) was extremely difficult due to how obscurely hard manipulating (and understanding) a .wav's elements are, especially as a newbie to the audio world.

At one point, calling a print statement or concatenating a number would make the program slow to almost an infinite loop, while commenting it out made it work perfectly.

Accomplishments that I'm proud of
I did not use any outside references to come up with this idea nor implement it - except the NAudio API and related samples/tutorials that I referenced in order to properly learn the library.

What we learned
NAudio is quite expansive, and audio in general has a depth and complications to it that takes a very long time to understand.

What's next for TuneCrypter-bitcamp16
Further fine-tuning, research on better algorithms and efficiency. Figure out more about how .wav (and other audio formats) store/present their information, in depth this time.

Built With
visual-studio
c#
windowsformapplication
naudio
wave
wavefilewriter
.net
audiointerface

C# encryption/decryption module created by Joseph Schiarizzi
