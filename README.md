Rabbit stream cipher implementation http://tools.ietf.org/rfc/rfc4503.txt   
> Rabbit is a stream cipher algorithm that has been designed for high
> performance in software implementations.  Both key setup and
> encryption are very fast, making the algorithm particularly suited
> for all applications where large amounts of data or large numbers of
> data packages have to be encrypted.  
 
Usage:
```java
    byte[] msg = "Hello World!".getBytes();
    RabbitCipher cipher = new RabbitCipher();
    cipher.setupKey(key);
    cipher.crypt(msg);
```

Currently IV usage not implemented.
