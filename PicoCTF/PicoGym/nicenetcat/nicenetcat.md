# PicoGYM Nice netcat...
> Accessed 5 October 2022
**15 POINTS**
---

## Description
>There is a nice program that you can talk to by using this command in a shell: $ **nc mercury.picoctf.net 21135**, but it doesn't speak English...
---

## Hints
1.  You can practice using netcat with this picoGym problem: [what's a netcat?](https://play.picoctf.org/practice/challenge/34)
2.  You can practice reading and writing ASCII with this picoGym problem: [Let's Warm Up](https://play.picoctf.org/practice/challenge/22)
---

## Explanation

When accessing the given command in shell "**nc mercury.picoctf.net 21135**" we will get an output of several number like this:

![Output Command](/PicoCTF/PicoGym/nicenetcat/Capture.PNG)
---
```python
octal =[112 ,105 ,99 ,111 ,67 ,84 ,70 ,123 ,103 ,48 ,48 ,100 ,95 ,107 ,49 ,116 ,116 ,121 ,33 ,95 ,110 ,49 ,99 ,51 ,95 ,107 ,49 ,116 ,116 ,121 ,33 ,95 ,97 ,102 ,100 ,53 ,102 ,100 ,97 ,52 ,125 ,10]
test = ""

for i in octal:
    test += chr(i)

print(test)
```
![Program](/PicoCTF/PicoGym/nicenetcat/nicenetcat.py)
