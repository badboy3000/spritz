
A C implementation of [Spritz](http://people.csail.mit.edu/rivest/pubs/RS14.pdf),
a spongy RC4-like stream cipher and hash function.

```c
int spritz_hash(unsigned char *out, size_t outlen,
                const unsigned char *msg, size_t msglen);

int spritz_stream(unsigned char *out, size_t outlen,
                  const unsigned char *key, size_t keylen);

int spritz_encrypt(unsigned char *out, const unsigned char *msg,
                   size_t msglen, const unsigned char *key, size_t keylen);

int spritz_decrypt(unsigned char *out, const unsigned char *msg, size_t msglen,
                   const unsigned char *key, size_t keylen);
```

