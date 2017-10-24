# USING MAC OS or Linux

# Open a new terminal.

# Step 1: Using the SSH-KEYGEN

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

## Step 2: Copy Public Key to VM

```
sudo cat ~/.ssh/gcp_deeplearn_gpu.pub
```

## Copy this entire key to GCP ssh key

<kbd>
  <img src="/MAC_LINUX_2_cat_pub_key.png">
</kbd>

## Once you've copied your key, continue from [Step 6](https://github.com/s3p02/gcp_console_getting_started)


# USING WINDOWS (Putty)

[Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) putty for windows.

# Step 1: Installation

## Click 'Next'. 

<kbd>
  <img src="/0_putty_install.PNG">
</kbd>

## Click 'Next'. 

<kbd>
  <img src="/1_next.PNG">
</kbd>

## Click 'Install'. 

<kbd>
  <img src="/2_install.PNG">
</kbd>

## Click 'Finish'. 

<kbd>
  <img src="/3_finished.PNG">
</kbd>

# Step 2: Generate SSH Key using PuTTYgen

## From the start Menu, search for putty and click 'PuTTYgen'. 

<kbd>
  <img src="/4_putty_gen.png">
</kbd>

## Click 'Generate'.

<kbd>
  <img src="/5_generate.PNG">
</kbd>

## Move your mouse cursor on the blank area, to generate some randomness.

<kbd>
  <img src="/6_move_over_blank_area.PNG">
</kbd>

## Replace the Key comment, with your GCP username.

<kbd>
  <img src="/7_replace_with_user_name.PNG">
</kbd>

## Copy the entire public key contents as highlighted.

<kbd>
  <img src="/8_copy_contents.PNG">
</kbd>

## You can save your public and private key for future reference. You can give a passphrase for your keys if you want. Since I haven't I will be prompted to do so later while saving the private key.

## Click 'Save public key'.

<kbd>
  <img src="/9_save_public_private_key.PNG">
</kbd>

## Name you file and click 'Save'.

<kbd>
  <img src="/10_pub.PNG">
</kbd>

## Click 'Save private key'.

<kbd>
  <img src="/9_save_public_private_key.PNG">
</kbd>

## Since I never gave a passphrase, I can click 'Yes'.

<kbd>
  <img src="/11_private_yes.PNG">
</kbd>

## Name you file, make sure it's not same as your public key and click 'Save'.

<kbd>
  <img src="/12_private.PNG">
</kbd>

## Once you've copied your key, continue from [Step 6](https://github.com/s3p02/gcp_console_getting_started), you can save your key as well with the following steps.

# Step 3: Launch PuTTY

## You can obtain your public IP address by returning to your GCP console.

<kbd>
  <img src="/14_ip_address.PNG">
</kbd>

## From the start Menu, search for putty and click 'PuTTY'. 

<kbd>
  <img src="/13_start_putty.png">
</kbd>

## 1. Scroll down.
## 2. Click 'Connection'
## 3. Click 'SSH'
## 4. Click 'Auth'
## 5. Click 'Browse' and select the private key you save from PuTTYgen, which has a extension '.ppk'


<kbd>
  <img src="/15_ssh_auth_browse_private_key.PNG">
</kbd>

## 1. Scroll back up, Click 'Session'
## 2. Enter your public ip address
## 3. name your session
## 4. Click 'Save'
## 5. Start your session by clicking 'Open'

<kbd>
  <img src="/16_save.PNG">
</kbd>

## Security Alert

# Click 'yes' when prompted.

<kbd>
  <img src="/security_alert.JPG">
</kbd>

## Enter your GCP username and hit the 'Enter/return' key to login to your VM

<kbd>
  <img src="/17_login_as.PNG">
</kbd>
