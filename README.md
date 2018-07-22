# homeworkjuly20

Create SSH Key Pair in Bash:

id_rsa -- private key
ida_rsa.pub -- public key (the lock)

Your local machine uses SSH to connect to AWS

Amazon web services --> EC2
Create instance --> launch instance
Step 1: Choose an Amazon Machine Image (AMI) --> Ubuntu Server 16.04 LTS (HVM) -- FREE TIER ELIGIBLE
Step 2: General Purpose t.2 micro -- FREE TIER ELIGIBLE
Step 3: Configure instance -- skip to leave default settings
Step 4: Add storage --> edit size from 8 GB to 20 GB (30 GB is free as of 7/18)
Step 5: Add Tags --> skip to leave default settings
Step 6: Configure Security Group --> Select existing security group (the one you made earlier)

Provisioning Docker Instance on AWS in Bash:

<code>curl - sSL https://get.docker.com | sh
sudo usermod – aG docker Ubuntu</code>

$ ssh ubuntu@<IP>


Pwnage: change port from 27017 default to 27016
