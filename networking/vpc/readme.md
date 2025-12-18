# FROM CONSOLE 
![alt text](scs/step1.png)

***Choose Name and IPV4 CIDR***

![alt text](scs/step2.png)
# FROM CLI
***aws ec2 create-vpc \\***<br>
  ***--cidr-block 10.0.0.0/16 \\***<br>
  ***--tag-specifications 'ResourceType=vpc,Tags=[{Key=Name,Value=my-vpc}]'***

![alt text](scs/step3.png)
# DONE
![alt text](scs/step4.png)