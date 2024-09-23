# Argonis: Open-Source Vulnerability Scanner 🔍

## Project Overview
Argonis is an open-source vulnerability scanner designed to detect and report security vulnerabilities within IT systems and applications. Its main goal is to provide businesses and developers with a powerful and flexible tool to scan their resources, generate reports, and manage alerts in a centralized way.

## Key Features (MVP)
- **Vulnerability Scanning:** A built-in scanning engine capable of detecting a wide range of vulnerabilities in systems and applications.
- **Asynchronous Task Management:** Leverages Celery and RabbitMQ to orchestrate background scans and tasks without affecting system performance.
- **Centralized Results Storage:** Securely stores scan results, users, and configurations in a PostgreSQL database.
- **Elasticsearch Integration:** Provides fast indexing of vulnerabilities and scan results for efficient search and analysis.
- **Notification System:** Generates and sends alerts via email, webhook, or other configured channels when critical vulnerabilities are detected.
- **Report Generation:** Automatically creates scan reports in various formats (PDF, JSON) for easy tracking of results.
- **API Authentication:** Robust authentication management using OAuth or JWT to secure access to resources and results.

## Deployment and Availability 
- **Self-hosted:** Designed for on-premises or private cloud deployment in enterprise environments. 
- **Open Source:** Free and open for community contributions. 
- **Flexible Deployment Options:**
  - Standard installer for traditional setups.
  - Docker container provided for easy deployment and scaling (Kubernetes-friendly).

## Architecture
Argonis employs a modular, scalable architecture designed for flexibility and performance. It connects various components to manage vulnerability scanning, task orchestration, and reporting.

![Architecture drawio](https://github.com/user-attachments/assets/27fdaa6c-c378-466a-afba-af2a1b445f69)

## Workflow
- **Scanning:**
Users trigger scans manually via the API or set up scheduled scans.
Results are indexed in PostgreSQL and Elasticsearch for fast search and processing.
- **Task Management:**
Celery Workers handle scans in the background, orchestrated by RabbitMQ to ensure smooth execution even at large scale.
- **Report Generation:**
Upon scan completion, detailed reports are automatically generated and can be downloaded or accessed through the API.
- **Notifications:**
When critical vulnerabilities are detected, users are notified via email, webhook, or other configured channels.
- **Data Analysis:**
Elasticsearch enables quick search and analysis of scan results to facilitate the review of vulnerabilities.

## Roadmap

### Immediate Post-MVP Plans:
- **Enhanced Dashboard:** Implement an interactive dashboard for visualizing vulnerability trends.
- **Scheduler Integration:** Add the ability to schedule automatic scans with specific configurations.

### Future Enhancements:
- **External Vulnerability Feeds:** Integrate with external databases (CVE, NVD) to enrich scan results.
- **Machine Learning Insights:** Implement machine learning models to automatically classify vulnerabilities by severity.
- **Integration with CI/CD Tools:** Connect Argonis with CI/CD pipelines to automate scans during deployments.
