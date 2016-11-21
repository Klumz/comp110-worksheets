### a)
```
s2 = 0
s3 = 0

while s3 != 0:
  s2 += s1
  s3 -= 1
```

### b) 
Because s2's value increases depending on s1's value, meaning that it would be multiplied by s1, s0 times.

### c)
```
s0 = 10
s1 = 1

while s0 != 0:
  s2 = 0
  s3 = s0
  while s3 != 0:
      s2 += s1
      s3 -= 1
  s1 = s2
  s0 -= 1
```

### e)     
```
       addi $s0, $zero, 10
       addi $s1, $zero, 1
inner: mult $s1, $s0
       mflo $s1
       addi $s0, $s0, -1
       bne $s0, $zero, inner
```
