### Configuration ( ~/.radare2rc)
```
e scr.utf8=true
e scr.utf8.curvy=true
e asm.cmt.right=true
eco solarized
```

### Configuration (./somefile.rr2) , Useful when we want to automate some input from stdin through file. So if any input is required, the value will be fetched from here
```
#!/usr/bin/rarun2
stdin=./exploit
stdout=./outfile
```

### utilization
```
r2 -r .somefile.rr2 -d binary
```

### Basic Functions
```
View all symbols  - afl
View all function - pdf @ sym.main
RunTillBreakPoint - dcu 0xAddress
StepOver          - S
VisualMode - V
Cycle Through VisualModes - p
```
