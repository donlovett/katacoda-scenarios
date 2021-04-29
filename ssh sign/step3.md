Step 3

Let's get a little bit creative and add something to our text and use 2 in the text file

Let's confirm the hash value or digest of the new file

```
openssl dgst hello.txt
```{{execute}}

You now ready to sign the text file hello.txt with your ssh key

We can put .sig to indicate the signed version

```
cat hello.txt | ssh-keygen -Y sign -n file -f ssh-key-test > hello.txt.sig
```{{execute}}

To see all of the options for this command you can enter the manual (man) option

```
ssh-keygen man
```{{execute}}

Ok Great|  That was awsome Let's finish up by valadating our signed file called hello.txt.sig 

```
cat hello.txt | ssh-keygen -Y check-novalidate -f ssh-key-test -n file -s hello.txt.sig
```{{execute}}

Wow - You did it.  Let's contiune to the next page for a summary of what you just accomplished.