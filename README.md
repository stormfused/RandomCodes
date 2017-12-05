# RandomCodes

### Python
#### Read Online File
```
#! /usr/bin/env python

try:
    # For Python 3.0 and later
    from urllib.request import urlopen
except ImportError:
    # Fall back to Python 2's urllib2
    from urllib2 import urlopen

html = urlopen("http://www.google.com/") # .read().decode('utf-8')
# html = html.read().decode('utf-8')
print(html.read())
```
```
#! /usr/bin/env python

import time
try:
    # For Python 3.0 and later
    from urllib.request import urlopen
except ImportError:
    # Fall back to Python 2's urllib2
    from urllib2 import urlopen

while True:
    html = urlopen("https://www.manager.io/version.txt") # .read().decode('utf-8')
    html = html.read().decode('utf-8')
    if html != "17.12.2":
        print("Version Changed: ")
        html2 = urlopen("https://api.telegram.org/bot477758678/sendmessage?text=New%20Version:%20" + ht
    print("No Changes")
    time.sleep(10)

``
