# USING MAC OS or Linux

Open a new terminal.

# Step 1: Using the SSH-KEYGEN

```
sudo ssh-keygen -t rsa -f ~/.ssh/gcp_deeplearn_gpu -C srpa3180
```
Here I have named my key 'gcp_deeplearn_gpu' located in '~/.ssh/' and 'srpa3180' is my username

<kbd>
  <img src="/MAC_LINUX_0_ssh_keygen.png">
</kbd>

You can enter a passphrase if you'd like or leave it blank by just hitting Enter/return key

<kbd>
  <img src="/MAC_LINUX_1_path_2_key.png">
</kbd>

Location to your public key is as highlighted above in red, and can be accessed with the following cat command in Step 2.

# Step 2: Copy Public Key to VM

```
sudo cat ~/.ssh/gcp_deeplearn_gpu.pub
```

Copy this entire key to GCP ssh key

<kbd>
  <img src="/MAC_LINUX_2_cat_pub_key.png">
</kbd>


# USING WINDOWS (Putty)

[Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) putty for windows.

# Step 1: Installation

Click 'Next'. 
<kbd>
  <img src="/0_putty_install.PNG">
</kbd>

Click 'Next'. 
<kbd>
  <img src="/1_next.PNG">
</kbd>

Click 'Install'. 
<kbd>
  <img src="/2_install.PNG">
</kbd>

Click 'Finish'. 
<kbd>
  <img src="/3_finished.PNG">
</kbd>


