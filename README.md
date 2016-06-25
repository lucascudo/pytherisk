# pytherisk
A Python toolset to develop Asterisk AGI scripts.

## Installing
```sh
pip install gTTS
```

## Using
Just copy pytherisk.py to your AGI script directory and import it. Example:
```python
#!/usr/bin/python

import pytherisk

pytherisk.speak("Olá, você ligou para ACM ltda. Digite o ramal desejado")
ramal = pytherisk.wait_for_digit(10000) # wait a digit for ten seconds
pytherisk.transfer("SIP", ramal) or pytherisk.busy()
