Let's confirm where we are

Rather than type the commands on the right part of the screen - Just click on the symbol at the end of the command.

First practice

uname -a tells us a bit about the resource that we are connected to

```
uname -a
```{{execute}}

Ok Great|  Let's move to our command to create our key.
We are going to execute the ssh We are going to use two handy options that you can learn more about by scrolling down if you are interested.

Let's give it a try.  

Remember that you can just click on the return symbol on the left screen instead of typing on the right console.

```
ssh-keygen -f ssh-key-test -C "This is an SSH key generation test" -N ""
```{{execute}}


Great Job!
Notice the output shows the naming for both keys

Next step is to save some text to a file that we can sign

```
echo "Hello World" > hello.txt
```{{execute}}



Perfect!

Let's keep going.


the -f command gives us the chance to specify a filename.  We want to do this since most systems already have keys in place that we do not want to overwrite.

The -C command allows us to add a comment to the key which could come in handy later.
