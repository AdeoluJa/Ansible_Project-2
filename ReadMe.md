# **ANSIBLE PROJECT 2**

## __Using Ansible To Deploy__
<li> Using Ansible Playbook in the host instance created (this was created using the VPC which was used to create the private instances) Nginx, PHP and PHP configurations where deployed in the private instances (with the help of the NAT Gateway the priavte instances where able to access  the internet).

<br>

*See the screenshot below*
<br>
![yaml file](./images/yaml1.png)
![yaml file](./images/yaml2.png)
<br>
<br>

## __AWS__

### __*Created VPC*__
<li> VPC created with the avialable subnets, and route tables for both  private and public use for EC2 instances.

<br>

*See the screenshot below*
<br>
![VPC](./images/1.png)
<br>
![Subnet](./images/2.png)
<br>
![RouteTable](./images/3.png)
<br>
<br>

### __*NAT Gateway*__
<li> This was created so that the private instances can reach the internet and deploy updates or installing nginx and php.

<br>

*See the screenshot below*
<br>
![NAT Gateway](./images/Nat.png)

*But was deleted due to the AWS charge assoicated to it*
<br>
<br>

### __*EC2 Instances*__
<li> NginxServer1 and NginxServer 2 are the private instances created under the VPC created and the host is the public instance created under the VPC so that the private instances can be viewed, use the NAT Gateway and also how the ansible playbook was ran. 

<br>

*See the screenshot below*
<br>
![EC2 Instance](./images/Instances.png)
<br>
<br>

### __*Target Group*__
<li> Shows the target group and health status of the registered private instances

<br>

*See the screenshot below*
<br>
![Target Group](./images/target.png)

<br>
<br>

### __*Load Balancer*__
<li> Displays the content of the private instances registered to the target groups and displays either of the content at a time.

<br>

*See the screenshot below*
<br>
![Load Balancer](./images/load.png)

<br>
<br>

### __*Content Load Balancer Display*__
<li> Shares the load between them and the displays either at a time.

<br>

*See the screenshot below*
<br>
![Server1](./images/server1.png)
![Server2](./images/server2.png)
<br>
