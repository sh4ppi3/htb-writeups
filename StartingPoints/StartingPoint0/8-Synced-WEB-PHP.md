# Recon

![Pasted image 20260805004504.png](../../Images/Pasted%20image%2020260805004504.png)

# FootHold

Rsync is **a** service that can **synchronize a directory** of yours with **a** remote **directory**. For us, **it** is **interesting** because we can see what files they have on their side.

You can use `$target::` to connect via **the** default port 873.  
Or `$target:` to connect via **the** SSH port 22, but you would need authentication.

`rsync --list-only $target::`

![Pasted image 20260805004830.png](../../Images/Pasted%20image%2020260805004830.png)

Lets see whats in public

`rsync --list-only $target::public`

![Pasted image 20260805005224.png](../../Images/Pasted%20image%2020260805005224.png)

# Flag

Now, lets get the flag from their repository

![Pasted image 20260805005515.png](../../Images/Pasted%20image%2020260805005515.png)

