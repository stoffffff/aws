# FROM CONSOLE
![alt text](scs/step1.png)

***Choose the actions to allow or deny***<br>

![alt text](scs/step2.png)

***Choose the name and description of your policy***<br>

![alt text](scs/step3.png)
# FROM CLI
***aws iam create-policy \\***<br>
  ***--policy-name business-analyst-policy \\***<br>
  ***--policy-document file://ec2-readonly-policy.json \\***<br>
  ***--region us-east-1***

***CONTENT of ec2-readonly-policy.json ***<br>
***{***<br>
  ***"Version": "2012-10-17",***<br>
  ***"Statement": [***<br>
    ***{***<br>
      ***"Effect": "Allow",***<br>
      ***"Action": [***<br>
        ***"ec2:Describe*"***<br>
      ***],***<br>
      ***"Resource": "*"***<br>
    ***}***<br>
  ***]***<br>
***}***<br>
