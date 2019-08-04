### paramiko
---
https://github.com/paramiko/paramiko

http://www.paramiko.org/

```py
import base64
import paramiko
key = paramiko.RSAKey(data=base64.b64decode(b'AAA...'))
client.get_host_keys().add('shh.example.com', 'ssh-rsa', key)
client.connect('shh.example.com', username='strongbad', password='thecheat')
stdin, stdout, stderr = client.exec_command('ls')
for line in stdout:
  print('... ' + line.strip('\n'))
client.close()

```

```sh
pip install paramiko

pip install -r dev-requirements.txt
pytest
pip install -r dev-requirements.txt
pip install k5test gssapi pyasn1
pytest
```

```
```


