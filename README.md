# Create SSH key


## I. USING MAC OS or Linux

Open a new terminal.

## Step i: Using the SSH-KEYGEN

```
sudo ssh-keygen -t rsa -f ~/.ssh/gcp_deeplearn_gpu -C srpa3180
```
## Here I have named my key 'gcp_deeplearn_gpu' located in '~/.ssh/' and 'srpa3180' is my username

<kbd>
  <img src="/MAC_LINUX_0_ssh_keygen.png">
</kbd>

## You can enter a passphrase if you'd like or leave it blank by just hitting Enter/return key

<kbd>
  <img src="/MAC_LINUX_1_path_2_key.png">
</kbd>

## Location to your public key is as highlighted above in red, and can be accessed with the following cat command in Step 2.

## Step ii: Copy Public Key to VM

```
sudo cat ~/.ssh/gcp_deeplearn_gpu.pub
```

## Copy this entire key to GCP ssh key

<kbd>
  <img src="/MAC_LINUX_2_cat_pub_key.png">
</kbd>

## Once you've copied your key, continue from [Step 6](https://github.com/s3p02/gcp_console_getting_started)


## II. USING WINDOWS (Putty)

[Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) putty for windows.

## Step i: Installation

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

## Step ii: Generate SSH Key using PuTTYgen

 From the start Menu, search for putty and click 'PuTTYgen'. 

<kbd>
  <img src="/4_putty_gen.png">
</kbd>

Click 'Generate'.

<kbd>
  <img src="/5_generate.PNG">
</kbd>

Move your mouse cursor on the blank area, to generate some randomness.

<kbd>
  <img src="/6_move_over_blank_area.PNG">
</kbd>

Replace the Key comment, with your GCP username.

<kbd>
  <img src="/7_replace_with_user_name.PNG">
</kbd>

Copy the entire public key contents as highlighted.

<kbd>
  <img src="/8_copy_contents.PNG">
</kbd>

## You can save your public and private key for future reference. You can give a passphrase for your keys if you want. Since I haven't I will be prompted to do so later while saving the private key.

Click 'Save public key'.

<kbd>
  <img src="/9_save_public_private_key.PNG">
</kbd>

Name you file and click 'Save'.

<kbd>
  <img src="/10_pub.PNG">
</kbd>

Click 'Save private key'.

<kbd>
  <img src="/9_save_public_private_key.PNG">
</kbd>

Since I never gave a passphrase, I can click 'Yes'.

<kbd>
  <img src="/11_private_yes.PNG">
</kbd>

## Name you file, make sure it's not same as your public key and click 'Save'.

<kbd>
  <img src="/12_private.PNG">
</kbd>

## Once you've copied your key, continue from [Step 6](https://github.com/s3p02/gcp_console_getting_started), you can save your key as well with the following steps.

 [Back to Main](https://github.com/s3p02/jupyter_gcp_nvidia-docker_digits/blob/master/README.md)
