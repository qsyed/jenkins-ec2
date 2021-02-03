# jenkins-ec2


## These are the steps and resource used to get an jenkins sever running on an Amazon EC2 instances.


> The first step is to launch an ec2 server in a public subnet so that the server has access to the internet. 
While in the securtity group section of launch the ec2. make sure you open ports 8080(for jenkins) and 22 (ssh) for yourself.

<img src = "images/sg-public.png">


>the next step is to connect to your instance via ssh, and run the following commands

* sudo yum update –y  (this updates the software on your instance)

* sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo   (this get the jenkins repo onto your server)

> the expect output should be following:
<img src = "images/jenkins-repo.png">



* sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
> their should be no output if done coorrectly 





