# Jenkins

What is Jenkins

Jenkins is widely employed as a crucial CI/CD tool for automating software development processes. Teams utilize Jenkins to automate building, testing, and deploying applications, streamlining the development lifecycle. With Jenkins pipelines, developers can define, version, and execute entire workflows as code, ensuring consistent and reproducible builds. Integration with version control systems allows Jenkins to trigger builds automatically upon code changes, facilitating early detection of issues and enabling teams to deliver high-quality software at a faster pace. Jenkins' flexibility, extensibility through plugins, and support for various tools make it a preferred choice for organizations aiming to implement efficient and automated DevOps practices.

## Getting started with Jenkins.
**Lets dive into installing Jenkins**


```
# Update package repositories
sudo apt update

# Install JDK (headless)
sudo apt install -y default-jdk-headless

# Install Jenkins
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update
sudo apt-get install jenkins

```

**Check if Jenkins has been installed, and its up and running.**
```
sudo systemctl status jenkins

```
<img width="964" height="393" alt="jenkin1" src="https://github.com/user-attachments/assets/b1a6d5cf-13d4-4e83-94b4-e4958f5b455a" />

Create an Instance "Jenkins" , with a new inbound rules for port 8080 in security group

By default, jenkins listens on port 8080, we need create an inbound rule for this in the security group of our jenkins instance.

<img width="695" height="187" alt="image" src="https://github.com/user-attachments/assets/b4815736-3cdc-47b5-9265-9b7960b946f0" />

**Set up Jenkins On The Web Console**

i. Input Jenkins Instance ip address on your web browser i.e. http://54.209.53.176:8080

ii. On your Jenkins instance, check "/var/lib/jenkins/secrets/initialAdminPassword" to know your password.

<img width="686" height="367" alt="image" src="https://github.com/user-attachments/assets/c88808cd-0dc6-4ed0-b60e-f080814383d2" />

iii. Install Jenkins pluggins

<img width="1278" height="700" alt="jenkins03" src="https://github.com/user-attachments/assets/d950e45c-d757-43c9-b907-0025812c2cc9" />

iv. Create a user account.

<img width="1347" height="682" alt="jenkins04" src="https://github.com/user-attachments/assets/21388d60-71e2-4a7e-8aa3-6c2847ac3f94" />

v. Log in to jenkins

<img width="693" height="320" alt="image" src="https://github.com/user-attachments/assets/a3dd7e3e-9301-4650-a7e7-20a0649a54af" />







