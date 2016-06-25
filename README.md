# pytherisk
A Python framework for communicating with Asterisk.

## Installing
```sh
pip install gTTS
```

##
Just copy pytherisk.py to your AGI script directory and import it. Example:
```python
#!/usr/bin/python

import pytherisk

pytherisk.speak("Olá, você ligou para Fulano. Aguarde enquanto direcionamos sua ligação.")
pytherisk.transfer("SIP", 666) or pytherisk.busy()