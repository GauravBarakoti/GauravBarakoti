<a href="https://gauravbarakoti.github.io/platform-engineering-portfolio/">
  <img src="assets/banner.jpg" alt="Gaurav Barakoti, DevOps Team Lead" width="100%" />
</a>

<div align="center">

### 👋 Hi, I'm Gaurav: DevOps Team Lead who wires frontends, backends, databases and clouds into platforms that ship fast and stay up.

[![Portfolio](https://img.shields.io/badge/💻_Open_my_portfolio-2ea043?style=for-the-badge)](https://gauravbarakoti.github.io/platform-engineering-portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gauravbarakoti)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bestgaurav1234@gmail.com)

</div>

```bash
gaurav@platform:~$ whoami
DevOps Team Lead @ Claudreck Technologies · AWS Certified Solutions Architect – Professional

gaurav@platform:~$ cat focus.yaml
cloud:        [AWS, GCP, DigitalOcean, Railway, Heroku]
containers:   [Docker, Docker Compose, Amazon ECS/ECR]
iac:          [Terraform (modules), Ansible]
ci_cd:        [GitHub Actions, CircleCI, Jenkins, AWS CodePipeline/CodeDeploy]
automation:   [n8n, Zapier, AWS Lambda, Python boto3]
data:         [Amazon RDS, PostgreSQL, MySQL, MS SQL, Redis, MongoDB]
connectivity: [AWS IAM, VPC, Security Groups, ALB/ELB, CloudFront, Cloudflare, DNS]
observe:      [CloudWatch, Sentry, Elasticsearch, Slack alerts]
```

---

### 🏗️ How I wire a production app, end to end

```mermaid
flowchart TB
    U([👤 Users]) --> CDN[Cloudflare / CloudFront · DNS · WAF · TLS]
    CDN --> LB[ALB / ELB]
    subgraph VPC["🔒 AWS VPC · private subnets · security groups"]
        direction TB
        LB --> FE[🖥️ Frontend · Vue / Next.js · 🐳 container]
        FE -->|REST / API| BE[⚙️ Backend API · Node / Python / PHP / Java · 🐳 ECS · Railway · DO]
        BE --> DB[(🗄️ RDS · PostgreSQL · MySQL · MS SQL · MongoDB)]
        BE --> R[(⚡ Redis cache)]
    end
    IAM{{🔐 AWS IAM · roles · least-privilege policies}} -.-> BE
    IAM -.-> DB
    CI[🔁 CI/CD · GitHub Actions · CircleCI · Jenkins] -->|docker build + push| ECR[(📦 Amazon ECR)]
    ECR -->|zero-downtime deploy| BE
    TF[🧱 Terraform + Ansible] -.->|provisions| VPC
    BE --> AUTO[🤖 n8n · Zapier · Lambda automations]
    BE --> MON[📈 CloudWatch · Sentry]
    AUTO --> SL[💬 Slack / email]
    MON --> SL
```

---

### 🛠️ Toolbox

**Cloud & PaaS**<br/>
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS" />
<img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" alt="GCP" />
<img src="https://img.shields.io/badge/DigitalOcean-0080FF?style=for-the-badge&logo=digitalocean&logoColor=white" alt="DigitalOcean" />
<img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white" alt="Railway" />
<img src="https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white" alt="Heroku" />

**Containers & IaC**<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Amazon_ECS%2FECR-FF9900?style=for-the-badge&logo=amazonecs&logoColor=white" alt="ECS/ECR" />
<img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" />
<img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white" alt="Ansible" />

**CI/CD**<br/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
<img src="https://img.shields.io/badge/CircleCI-343434?style=for-the-badge&logo=circleci&logoColor=white" alt="CircleCI" />
<img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" alt="Jenkins" />
<img src="https://img.shields.io/badge/CodePipeline_%2F_CodeDeploy-527FFF?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS CodePipeline / CodeDeploy" />

**Automation**<br/>
<img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n" />
<img src="https://img.shields.io/badge/Zapier-FF4A00?style=for-the-badge&logo=zapier&logoColor=white" alt="Zapier" />
<img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white" alt="AWS Lambda" />
<img src="https://img.shields.io/badge/Python_boto3-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python boto3" />

**Databases**<br/>
<img src="https://img.shields.io/badge/Amazon_RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white" alt="Amazon RDS" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
<img src="https://img.shields.io/badge/MS_SQL-CC2927?style=for-the-badge" alt="MS SQL" />
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />

**Connectivity & Security**<br/>
<img src="https://img.shields.io/badge/AWS_IAM-DD344C?style=for-the-badge&logo=amazoniam&logoColor=white" alt="AWS IAM" />
<img src="https://img.shields.io/badge/VPC_%26_Security_Groups-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="VPC & Security Groups" />
<img src="https://img.shields.io/badge/ALB_%2F_ELB-8C4FFF?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="ALB / ELB" />
<img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Cloudflare" />
<img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx" />

**Observability & OS**<br/>
<img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazoncloudwatch&logoColor=white" alt="CloudWatch" />
<img src="https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white" alt="Sentry" />
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white" alt="Elasticsearch" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />

---

### 🚀 Client work

| | | |
|---|---|---|
| 🟣 **[Optum](https://www.optum.com) · Dojo360** · 2024 – Present | Terraform development & **reusable Terraform modules** for the Dojo360 module | `Terraform` `IaC` |
| 🟢 **[Dashboard Lim](https://dashboard-lim.com)** · 2024 – Present | DevOps & cloud infrastructure for dashboards, API automations & AI tools | `Cloud` `Automation` |
| ✅ **[NewLIST](http://www.newlist.com)** · 2024 – 2025 | Test/stage/prod operations, Amazon Inspector remediation, CloudWatch everywhere | `Beanstalk` `CodePipeline` `WAF` `CloudFront` `RDS` |
| 🔵 **DigitalOcean → AWS** · 2026 | Led a production migration, scaling and memory-leak fixes at Shipway | `AWS` `DigitalOcean` `SRE` |
| 🟢 **Westminiter** | ECR → ECS with lazy loading for a 4 GB image; Terraform for EC2, IAM, S3, SQS, Bedrock, RDS | `Terraform` `Docker` `ECS` |

### 🧪 Hands-on labs (open source)

| Repo | What it shows |
|---|---|
| 🏛️ [**3TIER_ARCHITECTURE**](https://github.com/GauravBarakoti/3TIER_ARCHITECTURE) | Modular **Terraform** 3-tier AWS architecture: **VPC**, load balancer, Auto Scaling EC2, bastion host, **RDS** and S3 (web → app → database connectivity) |
| 🐳 [**vue.js-applicaition-dockerise**](https://github.com/GauravBarakoti/vue.js-applicaition-dockerise) | Dockerised Vue.js app → **ECR → ECS** behind **ELB / ALB** |
| 🔁 [**circleci-poc**](https://github.com/GauravBarakoti/circleci-poc) | **CircleCI** pipeline deploying an app with **zero downtime** |
| 🗄️ [**app-deployment-on-WindowsServer-using-Jenkins**](https://github.com/GauravBarakoti/app-deployment-on-WindowsServer-using-Jenkins) | Jenkins deploy of a .NET login app on Windows Server with an **RDS MS SQL** database |
| 🧱 [**aws-component-terraform**](https://github.com/GauravBarakoti/aws-component-terraform) | AWS resources provisioned with **Terraform** |
| 🚚 [**codeDeploy-AWS-python**](https://github.com/GauravBarakoti/codeDeploy-AWS-python) | Python app shipped with **AWS CodeDeploy** |
| ⚙️ [**ansibleWithJenkins**](https://github.com/GauravBarakoti/ansibleWithJenkins) | **Ansible** automation triggered from **Jenkins** |
| 🐍 [**boto-scripts**](https://github.com/GauravBarakoti/boto-scripts) · [**AWS-python-scripts**](https://github.com/GauravBarakoti/AWS-python-scripts) | **boto3** automation and audits across AWS services |
| 📊 [**cloudwatch-queries-for-dashboard**](https://github.com/GauravBarakoti/cloudwatch-queries-for-dashboard) | CloudWatch Logs Insights queries and dashboard widgets |

<a href="https://gauravbarakoti.github.io/platform-engineering-portfolio/#pipeline"><img src="assets/pipeline.jpg" alt="Interactive CI/CD pipeline from my portfolio" width="100%" /></a>

### 🏅 Certifications

![AWS SA Pro](https://img.shields.io/badge/AWS_Certified-Solutions_Architect_Professional-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![AWS SA Associate](https://img.shields.io/badge/AWS_Certified-Solutions_Architect_Associate-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![AWS CCP](https://img.shields.io/badge/AWS_Certified-Cloud_Practitioner-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)

---

<div align="center">

`$ terraform plan` → **Plan: 1 to add** (a DevOps lead for your platform), 0 to change, 0 to destroy.

[Portfolio](https://gauravbarakoti.github.io/platform-engineering-portfolio/) · [LinkedIn](https://www.linkedin.com/in/gauravbarakoti) · [bestgaurav1234@gmail.com](mailto:bestgaurav1234@gmail.com)

</div>
