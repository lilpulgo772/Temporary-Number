# Temporary-Number
Scrape Numbers and Messages from https://temporary-phone-number.com
## ⚙️Installation
```
pip install temporary-number
```
## 📚Examples
### Get Random Number
Code:
```py
import temporary_number

number = temporary_number.get_number()
print(number)
number2 = temporary_number.get_number(country="Finland")
print(number2)
```
Result:
```
+447893985537
+3584573983862
```
### Get Messages of Number
Code:
```py
import temporary_number

messages = temporary_number.get_messages("+447893985537")
for message in messages:
  print(f"{message.time} | From {message.frm}")
  print(message.content)
```
Result:
```
10 hours ago | From Google
G-188346 is your Google verification code.
13 hours ago | From +447717397317
22
13 hours ago | From +447470629193
02
15 hours ago | From WhatsApp ‎‫أدح أ ع لطت ال 94-92 : لب ص اخ ل ا ب سرت او دوك‬‎ ‎‫45 هي لعgLq1p5sV6‬‎
22 hours ago | From Google
G-975469 is your Google verification code.
22 hours ago | From Google
G-661261 is your Google verification code.
22 hours ago | From Google
G-278280 is your Google verification code.
22 hours ago | From Google
G-326555 is your Google verification code.
22 hours ago | From Google
G-384883 is your Google verification code.
23 hours ago | From Google
G-014594 ialah kod pengesahan Google anda.
1 day ago | From Amazon
002399 is your Amazon OTP. Do not share it with anyone.
1 day ago | From Google
G-102920 is your Google verification code.
1 day ago | From Google
G-525544 Google
1 day ago | From +447868655400
54340
...
```
