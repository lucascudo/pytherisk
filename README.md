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

pytherisk.speak("Olá, você ligou para Fulano. Aguarde enquanto direcionamos sua ligação.")
pytherisk.transfer("SIP", 666) or pytherisk.busy()
