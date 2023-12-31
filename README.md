# Metadata for EC2 instance 

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. Each EC2 instance comes with metadata that you can access to obtain information about the instance. This metadata is available at a well-known URL, which is accessible from within the instance. The base URL for EC2 instance metadata is (http://169.254.169.254/latest/dynamic/).

Instance Metadata:

instance-id: The unique identifier for the instance.
ami-id: The ID of the Amazon Machine Image used to launch the instance.
instance-type: The type of EC2 instance (e.g., t2.micro, m5.large).
local-hostname: The private DNS hostname of the instance.
public-hostname: The public DNS hostname of the instance.
local-ipv4: The private IPv4 address of the instance.
public-ipv4: The public IPv4 address of the instance.
mac: The MAC address of the instance's network interface

#Steps 
1. Create EC2 instace in linux AMI (free tier)
2. connect to that instance
3. sudo yum install python3
4. sudo yum install git
5. Clone the Metadata repository : git clone https://github.com/Hedsneh/Metadata.git
6. Install PIP environment : sudo pip3 install pipenv
7. cd  Metadata
8. Install the dependencies : pipenv install & pip3 install requests
9. run command : python3 get_metadata.py
