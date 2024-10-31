## CaptstoneProject - Introduction to Cloud Computing

## Tasks
## 1 Implement Version Control with Git
1.1 Initialize Git Respository
- Begin by creating a project directory named "MarketPeak_Ecommerce"
   - Asnwer: I start by inputing the code "mkdir MarketPeak_Ecommerce"
 ![Screenshot (39)](https://github.com/user-attachments/assets/68f05838-e4b2-44d2-b2a9-15a0eee270a1)
- Inside this directory, intialize a git repository to manage your version control.
   - Answer: I do this by going into the MarketPeak directory by entering the "cd MarketPeak_Ecommerce" and then initializing s repository with the "git init" command
 ![Screenshot (40)](https://github.com/user-attachments/assets/e18f1018-d9ef-43bf-a757-53ae0798b6bb)

1.2 Obtain and Prepare the E-commerce Website Template
- Download a Website Template
![Screenshot (42)](https://github.com/user-attachments/assets/1418428d-0fe2-4b35-bdca-59fdb41e7c93)
- Prepare the Website Template: Extract the downloaded template into your project directory "MarketPeak_Ecommerce"
![Screenshot (44)](https://github.com/user-attachments/assets/457df0bd-7cd3-426a-b9bb-c9253f9855be)

1.3 Stage and Commit the Template to Git
- Add your website files to the Git repository
   - Error: I encoutered an error when trying to add the files by incorrectly insterting a "git add." command
![Screenshot (45)](https://github.com/user-attachments/assets/87e773fa-5751-470f-8683-759665ea8829)
   - Answer: I rectified this by inserting a "git add ." command instead
![Screenshot (47)](https://github.com/user-attachments/assets/fef9e58c-41b9-4340-a75b-25226c35fc2e)
- Set your Git global configuration with your username and email.
![Screenshot (48)](https://github.com/user-attachments/assets/7e17a64d-d209-4bc0-aad8-75a7ca68f743)
- Commit your changes with a clear, descriptive message.
   - Error: I encountered an error when i inputed my git commit command without adding an " sign
![Screenshot (49)](https://github.com/user-attachments/assets/d11de128-7c26-4b13-b1cd-62fe6e5d14d3)
   - Answer: I rectified this by adding the " sign and the commit went through on git.
![Screenshot (50)](https://github.com/user-attachments/assets/dd2dc4d1-3517-4ce0-967a-e0542274b36a)

1.4 Push the code to your Github repository
- Create a Remote Repository on GitHub: Log into your GitHub account and create a new repository named "MarketPeak_Ecommerce".Leave the repository empty without initializing it with a README., .gitignore, or license.
![Screenshot (51)](https://github.com/user-attachments/assets/cd04e72d-8dfe-4c6c-a96b-2990591fe4b5)
- Link your Local Repository to GitHub: In your terminal, within your project directory, add the remote repository URL to your local repository configuration.
![Screenshot (53)](https://github.com/user-attachments/assets/65715c3c-3cef-478f-8657-de38c0794941)
- Push your code: Upload your local repository content on GitHub
   - Error: I encountered an error because i entered the command "git push -u main" instead of "git push -u origin main"
![Screenshot (54)](https://github.com/user-attachments/assets/23b23653-bbbc-48e7-9ebe-b84d884f2bdd)
   - Answer: I entered the correct command "git push -u origin main"
![Screenshot (56)](https://github.com/user-attachments/assets/757f45b4-48f5-42e2-8806-b53bda40868d)

## 2 AWS Deployment

2.1 Set Up an AWS EC@ Instance
- Log in to the AWS Management Console
- Launch an EC2 Instance using an Amazon Linux AMI
![Screenshot (58)](https://github.com/user-attachments/assets/e14f0165-98e4-4c06-b21c-73ac5681eeb9)
- Connect to the instance using SSH
   - Error: I wasnt able to connect to the instance because of the wrong command i entered, i didnt enter the IP address correctly.
![Screenshot (59)](https://github.com/user-attachments/assets/12186c22-6459-40f3-8ca7-c0c39eedb332)
   - Answer: I copied the ssh address from the EC2 Connect page and ensured it was the correct address
![Screenshot (60)](https://github.com/user-attachments/assets/f4de5a5d-3222-41d4-81c0-c2c8c84d02f5)

2.2 Clone the repository on the Linux Server
- HTTPS Method
   - Answer: I copied the link on github HTTPS section and used the "git clone" command on the terminal
![Screenshot (64)](https://github.com/user-attachments/assets/6bac1b24-4f4c-49a0-a977-bfb08be335fd)

2.3 Install a Web Server on EC2
- Install Apache web server on the EC2 instance.
   - Answer: I first update the server by inputing the command "sudo yum update -y". Secondly, i installed the Apache web server by using the command "sudo yum install httpd -y"
     ![Screenshot (65)](https://github.com/user-attachments/assets/4723258f-5a82-43c2-9c11-0626409d0ad4)

     Then after installing Apache, i start and enable the web server with the commands "sudo systemctl start httpd" and "sudo systemctl enable httpd"
     ![Screenshot (66)](https://github.com/user-attachments/assets/7241fb39-7821-4af1-9887-327f73c1b990)

2.4 Configure httpd for Website
- Prepare the Web Direcctory: Clear the default httpd web directory and copy MarketPeak Ecommerce website files to it.
   - Answer: I used the command "sudo rm -rf /var/www/html/" and copy the files with the command "sudo cp -r home/MarketPeak_Ecommerce /var/www/html/"
![Screenshot (67)](https://github.com/user-attachments/assets/071fdab7-5660-4288-b6d7-17811fd0178b)
- Reload httpd: Apply the changes by reloading the httpd service.
   - Answer: I used the command "sudo systemctl reload httpd"
![Screenshot (68)](https://github.com/user-attachments/assets/41b84be2-e66d-4507-9375-f9ae3800210f)




     















