## Using AWS Systems Manager

I completed an AWS lab where I used AWS Systems Manager to manage and automate tasks on an EC2 instance. I created an Inventory association in Fleet Manager to collect system and application metadata from a managed instance. I then used Run Command to remotely install a custom web application (Widget Manufacturing Dashboard) without needing SSH access. After deployment, I validated the application through the instance’s public IP.

I also used Parameter Store to create a configuration parameter (`/dashboard/show-beta-features`) that dynamically enabled additional features in the application. Refreshing the dashboard confirmed that the application was reading configuration values directly from Parameter Store. This lab strengthened my skills in remote instance management, automation, and configuration control using AWS Systems Manager.


<img width="911" height="440" alt="image" src="https://github.com/user-attachments/assets/35b55c14-faaf-461d-bd8a-0268cd6c090b" />
after creating parameter:
<img width="890" height="397" alt="image" src="https://github.com/user-attachments/assets/79b1f161-7add-4f78-98da-5ac9ade38fce" />

## Using AWS Session Manager

I used AWS Systems Manager Session Manager to securely access an EC2 instance without SSH, open ports, or key pairs. Through the browser-based shell, I verified the installed application files and used the AWS CLI inside the session to retrieve EC2 instance metadata and describe running instances. This demonstrated how Session Manager provides secure, auditable, and IAM‑controlled access to instances, offering a safer alternative to traditional SSH while maintaining full command-line functionality.

<img width="925" height="436" alt="image" src="https://github.com/user-attachments/assets/52b26448-4d4d-45f7-8116-4d5740a81a33" />
