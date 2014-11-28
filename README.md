onetimepad
==========

Implemented from [Mario Vilas](https://breakingcode.wordpress.com/2010/02/17/one-time-pad-encryption-in-python/):

Taken from [this website](https://breakingcode.wordpress.com/2010/02/17/one-time-pad-encryption-in-python/):

This is how we generate a one-time pad of any given size:

```
./otp.py generate test.key -s 1024
```

This is how to generate a one-time pad key the same size as file to convert (add -p to use /dev/random for more randomness+securrity):

```
./otp.py generate test.key conscience.txt -f
```

Encrypt a message then using:

```
./otp.py encrypt conscience.txt test.key conscience.crypto 
```

Decrypt using:

```
./otp.py decrypt conscience.crypto test.key conscience2.txt
```
