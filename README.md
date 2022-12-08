# Exam_2420
###### Cloue M.
---
# Setting up
#### Starting off, you need to create the following:
  - Create SSH-keygen
  - 2 Droplets
  - Adding users for both Droplets
---
## Creating SSH-keygen
  1. Open Windows terminal to generate and ssh key by typing ```ssh-keygen```
  2. It will ask you where you want to store you keygen. For example:
  - ```Enter file in which to save the key (/Users/USER/.ssh/id_rsa): /Users/USER/.ssh/DO2_key```
  - The directory ```/Users/USER/.ssh/DO2_key``` is where the ssh-keygen is stored.
  - Copy the DO2_key.pub: ```cat /Users/USER/.ssh/DO2_key.pub``` then highlight and copy.
  3. Go to you Digital Ocean account and under ```Settings > Security > SSH keys```, click Add ```SSH key```
  4. Paste the DO2_key.pub in SSH key content then name it ```DO2_key``` (or anything you want).
  5. Click ```Add SSH Key```.

---
## Setting up 2 Droplets
  1. On the left navigation bar, Under ```Projects```, select or create a project where you want to store you droplets.
  2. Once your project is created or selected, select ```Resources``` and click ```Get Started with a Droplet``` 
  3. Change the following settings:
  - Choose an image: ```Ubuntu 22.04(LTS) x64```
  - Choose a plan: (you can choose any plan you want) but in this case, let's choose the basic and cheapest ```Basic - Regular with SSD - $4/mo```
  - VPC Network: ```vpc-web``` (or the name of the vpc that you just created)
  - Authentication: SSH keys ```DO2_key``` (or the name of the SSH keygen that you just created)
  - Finalize and Create: 2 Droplets then name it ```ubuntu-1 and ubuntu-2``` for convinience.
  - Add tags: ```Web```
  4. Click ```Create Droplet```
---
