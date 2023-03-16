# CarRekognization
Recognizes any cars in the images and produces the output with confidence levels.

Step 1: Create your AWS Account by using link provided in Canvas.
Step 2: Open Learner’s Lab after creating AWS account & download the pem key and save the access key id and secret access key for future use.
Step 3: Press on Start Lab and once the AWS button has turned green, click on the AWS button to redirect to the AWS Management Console.
Step 4: Create 2 EC2 Instances and allow three ports: SSH, HTTP, HTTPS and make sure they are up and running.
Step 5: Once your jar files are ready, Open Terminal in Mac and go to the current directory where the jar files and pem key exists.
Step 6: Run “chmod 400 PemKey.pem” to secure the pem key before using it.
Step 7: Run “ssh -i PemKey.pem ec2-user@yourdnsaddress” to connect to your instance. You should open 1 Terminals for each instance as the dns changes for each instance. 
Step 8: Download Cyberduck in Mac, open connection to the instance 1 by using the dns address of instance 1 and pem key which you’ve downloaded earlier to establish a connection and share your CarRunnable.jar file once the connection is established.
Step 9: Now, open connection to the instance 2 and share your TextRunnable.jar file once the connection is established.
Step 10: After the files are uploaded, open the terminal and type ls command to check if the file is visible in your instance. 
Step 11: Use command “aws configure” and provide your aws acess key id and aws secret access key and the region as “us-east-1” as we the in this region and install java and maven using “sudo yum install java” and “sudo yum install maven” commands as we are using JAR files.
Step 12: Open the terminal of the first instance and run “java -jar CarRunnable.jar”. Once it runs successfully then go to step 13.
Step 13: Open the terminal of the second instance and run “java -jar TextRunnable.jar > output.txt” so that the output is saved in the text file.
Step 14: You can then check the recognized images and confidence levels.
