**Infrastructure as Code (IaC) with Terraform**

## 🚀 Objective

Provision a local Docker container using **Terraform**.

---

## 🧰 Tools Used

- Terraform
- Docker

---

## 📁 Project Structure

terraform-docker-app/

├── main.tf

├── apply-log.txt

├── README.md

## 📝 Steps Performed

### 1. ✅ Wrote Terraform Configuration

File: `main.tf`
- Pulled the official **nginx** Docker image.
- Created a container named `nginx-container`.
- Exposed container port `80` to host port `8081` (since `8080` is used by Jenkins).

### 2. ✅ Terraform Commands Used

terraform init            # Initialize the project

terraform plan            # See execution plan

terraform apply           # Apply infrastructure changes

tee                       # log the output

terraform destroy         # Tear down the infrastructure

🌐 Access the Container

**After applying the configuration, open your browser:**

http://localhost:8081
You’ll see the nginx default welcome page.

🧪 Verification

To confirm the container is running:

docker ps

🗑️ Clean Up

To remove the container:

terraform destroy -auto-approve

✅ Screrenshots :
<img width="1062" height="642" alt="image" src="https://github.com/user-attachments/assets/57bb154e-4a63-400f-937c-aaa044b2e7e6" />

<img width="971" height="323" alt="image" src="https://github.com/user-attachments/assets/d1772be8-3ff2-4dae-ad5b-98a2d2df8ed9" />

