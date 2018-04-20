## Run the executable with some customized arguments in the gdb shell
Method 1
```
(gdb) r `python -c 'print "A"* 40'`
Starting program: /home/dibyendu/Desktop/b0f/b0f.o `python -c 'print "A"* 40'`
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA[Inferior 1 (process 3324) exited with code 050]
```
Method 2 ( 
```
(gdb) r $(python -c 'print "A"* 40')
Starting program: /home/dibyendu/Desktop/b0f/b0f.o $(python -c 'print "A"* 40')
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA[Inferior 1 (process 3330) exited with code 050]
```
## Run system commands in the gdb shell
Method 1 : Run system commands
```
(gdb) shell python -c 'print "A"* 40'
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
```
Method 2: 
```
(gdb) !python -c 'print "A"* 40'
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
```
