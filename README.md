☁️ Cloud-Based File Storage System Using Bash & AWS CLI

This is a simple cloud-based file storage system — inspired by services like Dropbox and Google Drive — implemented using Bash scripting and AWS S3. It allows users to upload, download, list, and delete files from an S3 bucket, with support for logging and GitHub Actions automation.

---

🎯 Project Objectives

- ✅ Upload files to S3
- ✅ Download files from S3
- ✅ List files in S3
- ✅ Delete files from S3
- ✅ Track actions in a log file with timestamps
- ✅ Automate uploads using GitHub Actions

---

📁 Folder Structure

.
├── aws_cloud # Main folder containg  Bash script to interact with S3
├── actions.log # Log file (generated)
├── .github/
│ └── workflows/
│ └── s3_automation.yml # GitHub Actions workflow file
└── README.md # Project documentation

yaml
Copy
Edit

---

🚀 Getting Started

1️⃣ Prerequisites

- AWS account with S3 and IAM access
- AWS CLI installed and configured (`aws configure`)
- Git and GitHub setup

---

2️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
3️⃣ Make the Script Executable
bash
Copy
Edit
chmod +x ass4.sh
4️⃣ Run the Script
bash
Copy
Edit
./ass4.sh
Follow the on-screen options to:

Upload files

Download files

List files

Delete files

🪵 Logging Actions
Each action performed by the script is logged into actions-TIMESTAMP.log with the format:

ruby
Copy
Edit
YYYY-MM-DD HH:MM:SS - ACTION - FILE
Logs are also uploaded to the logs/ folder in your S3 bucket.

🔄 GitHub Actions Automation
This project includes a CI/CD pipeline using GitHub Actions:

Automatically runs the script when code is pushed to main

Uses AWS credentials stored as GitHub Secrets:

AWS_ACCESS_KEY_ID

AWS_SECRET_ACCESS_KEY

Workflow file: .github/workflows/s3_automation.yml

🔐 Security Considerations
IAM user is used instead of root credentials

S3 bucket public access is enabled only for demo purposes (not for production)

🧰 Technologies Used
🐧 Bash

🟦 AWS CLI

☁️ Amazon S3

🔐 AWS IAM

⚙️ GitHub Actions

👤 Author
Abdulhakeem Abdullah Mujahid (Skymate)
Cloud Security Intern | AWS Enthusiast
🔗 LinkedIn | 🌐 GitHub

📃 License
This project is for learning/demo purposes only.

---

✅ Next Steps

- Save this file as `README.md` in your project root.
- Commit and push it:

```bash
git add README.md
git commit -m "Add project README"
git push origin main
