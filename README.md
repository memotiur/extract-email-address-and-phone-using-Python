# extract-email-address-and-phone-using-Python

Extract email address and phone number from Any website.
Python Code
```
import urllib.request,re
f = urllib.request.urlopen("http://www.thehotelwindsor.com.au/")
s = f.read().decode('utf-8')
print(re.findall(r"\+\d{2}\s?0?\d{10}",s))
print(re.findall(r"[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,4}",s))
```
