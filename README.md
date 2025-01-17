# RDP-EC2-Connection

## Step 1 : Go to EC2 homepage [here](https://us-east-1.console.aws.amazon.com/ec2/home)

## Step 2 : Click Launch instance or go to instances(if already any instance exists)
![image](https://github.com/user-attachments/assets/b1d3d6a6-8bba-45cf-a759-72b2ab4bc97e)

## Step 3 : Give any name or tags for your instance (any name will work but use a good one to quickly identify)
![image](https://github.com/user-attachments/assets/003a3c08-6038-4372-8a8e-050afdc8d787)

## Step 4: Select OS (I'll go with windows, for linux distro it is more easy to get access to machine directly from AWS websites)
![image](https://github.com/user-attachments/assets/50d98b07-ec84-4317-82c5-b21edd140970)

## Step 5: Select a free tier machine image if you don't want to get charged
![image](https://github.com/user-attachments/assets/f920ed76-650d-4254-827e-4e6e594b212d)

## Step 6: Select instance type (go with default one if trying out, micro with 1 GB should be enough at the beginning)

![image](https://github.com/user-attachments/assets/39cb8102-5983-4444-9d8e-1470bac4985c)

## Step 7: Generate a key pair by giving any name, it will generate a .pem file using this .pem file you can access into EC2 machine from any computer

![image](https://github.com/user-attachments/assets/eaca4220-de8e-4b09-8246-665b984de2e0)


## Step 8: Create a security group. Make sure to enable check which says, allow RDP traffic from anywhere 0.0.0.0/0

![image](https://github.com/user-attachments/assets/a922572c-000f-4659-95f4-375fd7fe4e37)

## Step 9: Choose the max free storage available or you can choose as per your need but avoid consting
![image](https://github.com/user-attachments/assets/b6bddcaf-9008-4828-9c06-067ab1f34fcd)

## Step 10: Click Launch instance after reviewing summary(avoid advance details unless you're sure about something)

![image](https://github.com/user-attachments/assets/1ca685b3-fdda-4e36-bd07-8fb434cab5eb)


---

## Connecting EC2 instance using MacOS (in windows we can connect directly using remote desktop connection which comes pre-installed)

#### Step 1: Find a RDP software. I used [freerdp](https://www.freerdp.com/)

#### Step 2: Download [xquartz](https://www.xquartz.org/) open source software to run windows system on macOS. Without it we won't be able to run the windows and face issues like 

(failed to open display: :0, Please check that the $DISPLAY environment variable is properly set.)

#### Step 3: Run the command:
```
xfreerdp /v:<EC2-Public-IP> /u:Administrator /p:<Password>
xfreerdp /v:53.191.233.45 /u:Administrator "/p:FLV################"
```

#### You should be able to access the EC2 windows instance
![image](https://github.com/user-attachments/assets/0eb6269a-2062-4fd1-a069-8714c1b256c5)

Installing python on windows EC2 instance. Do whatever you want but remember that it only has 1GB ram and fewer GB storage, because you have used for free ;)


### Happy Coding
### A R
