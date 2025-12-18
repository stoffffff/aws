# FROM Console
***From ec2 - launch instance:<br>Choose the name and OS Image***

![alt text](sc/step1.png)
***Create or select an existing key-pair (your credentials to ssh to the machine)***

![alt text](sc/step2.png)<br>
***Select existing security group or create a new one then select it<br>Finally, click 'Launch' instance'***

![alt text](sc/step3.png)
# DONE
![alt text](sc/step4.png)
# FROM CLI
***aws ec2 run-instances \\***<br>
  ***--image-id 'YOUR_IMAGE_ID' \\***<br>
  ***--instance-type t2.micro \\***<br>
  ***--key-name 'YOUR_KEY_NAME' \\***<br>
  ***--security-group-ids 'YOUR_SG_ID' \\***<br>
  ***--subnet-id 'YOUR_SUBNET_ID' \\***<br>
  ***--associate-public-ip-address \\***<br>
  ***--count 1 \\***<br>
  ***--tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=viktor-from-cli}]'***

![alt text](sc/step6.png)
# DONE
![alt text](sc/step5.png)

