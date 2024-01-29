![image](https://github.com/petriQore/Securinets-2024-Darkest-Hour-CTF/assets/123587287/4a572e4c-ade6-4a6c-b785-59288bea8a17)

so much time spent trying to find out what a document ID is, but it was just a google docs ID.

we find this doc: 

![image](https://github.com/petriQore/Securinets-2024-Darkest-Hour-CTF/assets/123587287/ead12914-36ee-4d8f-933a-0e1bf8584663)

it has a mega link and a very long string.

we didn't know what that string meant so we googled it and we found out it was an svg image and it displays this:

![image](https://github.com/petriQore/Securinets-2024-Darkest-Hour-CTF/assets/123587287/d497a9ff-f8c7-4c99-a688-47c637045df7)

we use that as the mega password and we find an audio.txt file with base64

using [dcode](https://www.dcode.fr/base-64-encoding) we can convert that to an actual audio file

listening to it didn't yield anything, so we plugged it into audacity and viewed the spectrogram

![image](https://github.com/petriQore/Securinets-2024-Darkest-Hour-CTF/assets/123587287/8af4648a-b2d8-40b7-8b5f-50f5fce446f2)

that looks like a QR code!

let's mess with the spectrogram settings until we get something better

![image](https://github.com/petriQore/Securinets-2024-Darkest-Hour-CTF/assets/123587287/7322615c-a15f-4838-86bd-aee2d32967be)

it's still messed up and needs more cleaning but eventually scanning it will give the flag
