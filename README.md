The main purpose of this session is, How to use Ansible in AWS context.

Prerequisite:
Install boto library

Authentication with AWS-related modules is handled by either specifying your access and secret key as ENV or module argumnets.

For environmental variables
1. export AWS_ACCESS_KEY_ID='AK123'
2. export AWS_SECRET_ACCESS_KEY='abc123'

For storing these in a vars_file, ideally encrypted with ansible-vault:

![image](https://user-images.githubusercontent.com/49281318/91826635-7a85f580-ec5b-11ea-9a4b-41aa0e44733b.png)

Note that if you store your credentials in vars_file, you need to refer to them in each AWS-module. For example:

![image](https://user-images.githubusercontent.com/49281318/91826737-9e493b80-ec5b-11ea-8530-a61f6f5deb36.png)

We can also have a boto config file to access the creds and secrets. /etc/boto.cfg or ~/.aws/credentials


Architecture:

![image](https://user-images.githubusercontent.com/49281318/91942437-93a0ac00-ed18-11ea-91af-4ef5e4faa0bb.png)

Refernence:
![image](https://user-images.githubusercontent.com/49281318/92122487-1b6ddf80-ee19-11ea-8eca-16118a8af7a5.png)


