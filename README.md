# DevOps-Training-1.2
## High Availability exercise

Let`s put on practice the HA concept creating an ASG which will bring up N number of EC2 instances with a NGINX configured. Those instances will be behind of a ELB which will be deployed on a public subnet.


![elb](https://raw.githubusercontent.com/AbelGuti/DevOps-Training-1.2/master/images/elb.png)


### Considerations
 * The EC2 instances must be in private subnets.
 * The install/configure of the NGINX server must be from the User Data.
 * Create two security groups, one for the ELB and another of the instances.
 * Restrinc the traffic, dont let unused ports opened.