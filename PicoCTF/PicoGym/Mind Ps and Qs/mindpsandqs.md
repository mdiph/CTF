# Mind your Ps and Qs
> Accessed 5 October 2022
**20 POINTS**
---

## Description
>In RSA, a small e value can be problematic, but what about N? Can you decrypt this? [values](https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values)
---

## Hints
1.  Bits are expensive, I used only a little bit over 100 to save money
---

## Explanations
you can download the "values" file or do this command in shell:
`wget https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values`
Checking that the file is an ASCII text by doing this command:
`file values`
After that, we can use a command to display the inside of the file:
`cat values`
and the program will output like this:
![Values Output](/PicoCTF/PicoGym/Mind%20Ps%20and%20Qs/Asset/Capture.PNG)

With that, we can use a web decryption tools [Web Tools](https://www.dcode.fr/rsa-cipher) and input the values
---

## Output
`picoCTF{sma11_N_n0_g0od_13686679}`
