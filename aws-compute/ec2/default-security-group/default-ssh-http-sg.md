# From AWS Console
![alt text](scs/default-ssh-http-sg.png)
# DONE
![alt text](scs/default-ssh-http-sg-created.png)
# FROM CLI
# STEP 1 - Create the security group first, retrieve the desired VPC Id from console or using the CLI
***aws ec2 create-security-group \\***<br>
  ***--group-name test-sg \\***<br>
  ***--description "This is a testing security group" \\***<br>
  ***--vpc-id 'YOUR_VPC_ID***<br>
# STEP 2 - Now attach the rule 
***aws ec2 authorize-security-group-ingress \\***<br>
  ***--group-id 'YOUR_SG_ID' \\***<br>
  ***--protocol tcp \\***<br>
  ***--port 22 \\***<br>
  ***--cidr 0.0.0.0/0***<br>
# Another rule
***aws ec2 authorize-security-group-ingress \\***<br>
  ***--group-id 'YOUR_SG_ID' \\***<br>
  ***--protocol tcp \\***<br>
  ***--port 80 \\***<br>
  ***--cidr 0.0.0.0/0***<br>