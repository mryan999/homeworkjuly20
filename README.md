# homeworkjuly20

Create SSH Key Pair in Bash:<br>
<br>
<code>ssh-keygen -t rsa -C "your_email@example.com"</code><br>
id_rsa -- private key<br>
ida_rsa.pub -- public key (the lock)<br>
<br>
Your local machine uses SSH to connect to AWS<br>
<br>
Amazon web services --> EC2<br>
Create key pair --> choose whatever name --> paste public key<br>
Create instance --> launch instance<br>
Step 1: Choose an Amazon Machine Image (AMI) --> Ubuntu Server 16.04 LTS (HVM) -- FREE TIER ELIGIBLE<br>
Step 2: General Purpose t.2 micro -- FREE TIER ELIGIBLE<br>
Step 3: Configure instance -- skip to leave default settings<br>
Step 4: Add storage --> edit size from 8 GB to 20 GB (30 GB is free as of 7/18)<br>
Step 5: Add Tags --> skip to leave default settings<br>
Step 6: Configure Security Group --> Select existing security group (the one you made earlier)<br>

Provisioning Docker Instance on AWS in Bash:<br>

<code>curl - sSL https://get.docker.com | sh</code><br>
<code>sudo usermod – aG docker Ubuntu</code><br>
<br>
<br>
tmux<br>
<code>docker pull hello-world</code>-- to test<br>
<code>docker pull jupyter/datascience-notebook</code><br>
<code>docker run --rm -p 10000:8888 -e JUPYTER_LAB_ENABLE=yes -v "$PWD":/home/jovyan/work jupyter/datascience-notebook:e5c5a7d3e52d</code><br><br>

Accessing Jupyter Notebook:<br>
<code>{public IP listed on EC2}:443</code> 

<br>
Pwnage: change port from 27017 default to 27016 in security groups to avoiding crawling bots looking for default settings<br>
<br>
Linux on t2.large $67/mo<br>
Linux on m4.4xlarge $586/mo<br>
Linux on i3.4xlarge $914/mo
