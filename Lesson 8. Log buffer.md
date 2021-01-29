# Image implementation 

Surely, we can't work with infinitive file in shared memory. How do we manage it? 

# Log buffer 

Under the image abstraction lies a special data stucture **Log buffer**

let's see it on an example. 

we will offer the same amount of data again and again and take a look how Log buffer manages that 

<p align="center">
  <img src="/img/Log buffer offer.svg">
</p>

the size of the message is 300 bytes 

we create a regular file and split it on 3 the same pieses: 

<p align="center">
  <img src="/img/Log buffer overall.svg">
</p>

Now let's write to it! 

// here some explanations what's going on and what admin_action's are 

<p align="center">
  <img src="/img/Log buffer.gif">
</p>
