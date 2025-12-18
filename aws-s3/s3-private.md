# FROM CONSOLE
![alt text](scs/step1.png)

***Choose the name of the bucket***

![alt text](scs/step2.png)

***Block all public access***

![alt text](scs/step3.png)
# FROM CLI
***aws s3api create-bucket \\***<br>
  ***--bucket developer-bucket-cli \\***<br>
  ***--region us-east-1***

***aws s3api put-public-access-block \\***<br>
  ***--bucket developer-bucket-cli \\***<br>
  ***--public-access-block-configuration '{***<br>
    ***"BlockPublicAcls": true,***<br>
    ***"IgnorePublicAcls": true,***<br>
    ***"BlockPublicPolicy": true,***<br>
    ***"RestrictPublicBuckets": true***<br>
  ***}'***

![alt text](scs/step4.png)
# DONE
![alt text](scs/step5.png)

