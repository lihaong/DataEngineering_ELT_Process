# 🚀 ELT Pipeline: PostgreSQL and dbt Integration

## 🌟 Overview
This repository showcases a robust ELT (Extract, Load, Transform) pipeline designed to streamline your data workflows. Whether you’re managing raw datasets or preparing analytics-ready tables, this pipeline has you covered! 

### Key Highlights:
1. **Extract**: Pull raw data from a **source PostgreSQL** database.
2. **Load**: Store the data in a structured format in a **destination PostgreSQL** database.
3. **Transform**: Use the power of [dbt](https://www.getdbt.com/) to apply modular, reusable SQL transformations.

💡 Orchestrated with **Apache Airflow** and deployed in a **Dockerized environment**, this pipeline ensures simplicity, scalability, and repeatability.

---

## ✨ Features
- 🔄 **Automated Extract and Load**: Extract raw data and seamlessly load it into your destination database.
- 🔧 **Effortless Transformation**: Use dbt to create, test, and version SQL models.
- ⚙️ **Orchestration at Scale**: Manage complex workflows with Apache Airflow.
- 🐋 **Containerized Ecosystem**: All services run in isolated, self-contained Docker containers.
- 🌍 **Customizable**: Flexible enough to adapt to diverse datasets and workflows.

---

## 🛠️ Architecture
**Visual Overview**:
```plaintext
   +----------------+            +-----------------------+           
   | Source         |            | Destination           |           
   | PostgreSQL     |  --->      | PostgreSQL            |           
   +----------------+            +-----------------------+           
           |                               ^
           |                               |                    
    Extract & Load                Transform (dbt)                    
           |                               |                    
       Airflow Orchestration                
```

---

## 🚀 Getting Started

### Prerequisites
- 🐳 Docker & Docker Compose installed.
- 🔗 Basic knowledge of PostgreSQL, dbt, and Airflow.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/lihaong/MobileApp_Ngojek.git
   cd MobileApp_Ngojek
   ```
2. Start the services:
   ```bash
   docker-compose up --build
   ```
3. Access Airflow:
   - 🌐 URL: [http://localhost:8080](http://localhost:8080)
   - 🔑 Username: `admin`
   - 🔑 Password: `admin`

---

## 🌀 Workflow

### Extract and Load
Python scripts automate data extraction from the source PostgreSQL and load it into the destination PostgreSQL database.

### Transform
- Create **reusable SQL models** using dbt.
- Execute transformations to produce analytics-ready datasets.

### Orchestrate
Airflow DAGs manage the pipeline and ensure tasks run efficiently.

---

## 📂 Project Structure
```plaintext
.
├── airflow/
│   ├── dags/               # Airflow DAGs
│   ├── plugins/            # Custom Airflow plugins
├── custom_postgres/         # dbt models and profiles
├── elt_script/              # Python scripts for Extract and Load
├── docker-compose.yml       # Docker Compose configuration
└── README.md                # Project documentation
```

---

## 🌈 Customization
- **Extract and Load**: Update `elt_script` for different data sources or schemas.
- **Transform**: Modify dbt models in `custom_postgres/` to fit your needs.
- **Orchestrate**: Extend Airflow DAGs with additional tasks or dependencies.

---

## 🤝 Contributions
We welcome contributions from the community!  
Submit your ideas, enhancements, or bug fixes through issues or pull requests.

---

## 📧 Contact
📌 Created by **Muhammad Fajar Andikha**  
📬 Reach out at: [your-email@example.com](mailto:your-email@example.com)

---

## 📝 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

🌟 Happy ELT-ing! 🚀
```

This version adds icons, better formatting, and a lively tone to make your project more inviting and easier to navigate. Let me know if you'd like further tweaks!
