# multi-tier-web-app-provisioning
This project automates the provisioning and deployment of a multi-tier web application stack using various technologies such as MySQL, Memcached, RabbitMQ, Apache Tomcat, and Nginx. The infrastructure setup is designed for CentOS/RHEL-based systems, leveraging shell scripts to streamline the deployment process.

**Highlights:**
- Automated the entire setup process using shell scripts, ensuring consistent and repeatable deployments.
- Configured each component to work together seamlessly, providing a scalable and efficient environment for web applications.
- Demonstrated proficiency in managing and automating infrastructure using industry-standard tools and best practices.

**Outcome:**
This project provided valuable experience in DevOps practices, particularly in automating the deployment and configuration of complex multi-tier environments. The automated setup is ideal for development, testing, and demonstration purposes, showcasing a practical application of various open-source technologies.

## Project Structure
- **Vagrantfile:** Configuration for setting up virtual machines.
- **Scripts:** 
  - `backend.sh`: Sets up MySQL, RabbitMQ, and Memcached.
  - `tomcat.sh` and `tomcat_ubuntu.sh`: Installs and configures Apache Tomcat.
  - `nginx.sh`: Configures and sets up Nginx as a reverse proxy.
  - `rabbitmq.sh`: Automates the setup of RabbitMQ.
  - `mysql.sh`: Sets up and configures MySQL/MariaDB.
  - `memcache.sh`: Installs and configures Memcached.

## Setup Instructions

### Prerequisites
- **Vagrant:** Ensure Vagrant is installed on your system.
- **VirtualBox:** Install VirtualBox as the provider for Vagrant.

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/multi-tier-web-app-provisioning.git
   cd multi-tier-web-app-provisioning
2. **Start Environment:**
   ```bash
    vagrant up
3. **Provisioning Environment:**
- Vagrant will automatically execute the shell scripts to set up the multi-tier web application stack.
4. **Access the Application:**
- Once provisioning is complete, you can access the application through the Nginx server, which will proxy requests to the Tomcat application server, which would be the web01 IP address.
    ```bash
    cat etc/hosts
    ```

**Key Technologies:**
- **Vagrant:** To manage the virtual environment and automate the setup process.
- **Apache Tomcat:** Served as the application server for deploying Java web applications.
- **Nginx:** Configured as a reverse proxy and load balancer to optimize traffic distribution.
- **RabbitMQ:** Integrated as a message broker for handling asynchronous communication.
- **MySQL/MariaDB:** Deployed as the database server with secured access and initial data setup.
- **Memcached:** Implemented for caching to improve the performance of the database queries.

## License
[MIT License](LICENSE)

## Acknowledgments
This project was developed as part of the Udemy course "DevOps Projects" by Imran Teli. 

- **Course**: [DevOps Project](https://www.udemy.com/course-dashboard-redirect/?course_id=3710504) by Imran Teli

## Contact
For any inquiries, please reach out on [[LinkedIn](https://www.linkedin.com/in/oluwatobi-oni-22582159/)].



