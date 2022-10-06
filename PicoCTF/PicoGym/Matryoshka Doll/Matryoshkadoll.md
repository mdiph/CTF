# Matryoshka Doll
> Accessed 6 October 2022
**30 POINTS**

---

## Description 
>Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/b6205dd933ec01c022c4e6acbdf11116/dolls.jpg)
---

## Hints
1.  Wait, you can hide files inside files? But how do you find them?
2.  Make sure to submit the flag as picoCTF{XXXXX}
---

## Explanation
Like the name of the challenge, its a doll that have another doll inside it, the same as the challenge, first we need to download the **dolls.jpg** with the provided link or use this command:

`wget https://mercury.picoctf.net/static/b6205dd933ec01c022c4e6acbdf11116/dolls.jpg`

after that we can start unzipping the files, and it will contain several more .jpg file inside a directory called "base_iamges":

![List Directory](/PicoCTF/PicoGym/Matryoshka%20Doll/Asset/Capture.PNG)

and at the end of the directory, there will be a `flag.txt` that have the flag.

## Output
`picoCTF{4f11048e83ffc7d342a15bd2309b47de}`
