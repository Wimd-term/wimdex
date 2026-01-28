# wimdex
The structure of Wimd which it allows you to make your own extensions for Wimd and more stuff!

How to make my own extentions?

absoulotly we have structure on Wimd which you can use that structure on your app!

if you want use examples you need to make files like this:

* My project \
* main.py
  * extensions\
    * 001.py
    * ...

so lets code on it!

there is structure to send a request:
==main.py==

```python
import wimdex

input1 = input("input-> ") # to get input
input1 = wimdex.wimdsend(input1) # to send it [...]
wimdex.to(input1, "extensions") # send input1 to [... extensions folder]
```
absoulotly after this command it runs all files on extensions folder

# how to make my own extension?

so that code sent request so how to get output? if you want to make your own extension you need this code!
==001.py==
```python
import wimdex

message = wimdex.check()
if message == "hi":
    print("hello! this is 001.py")
```
