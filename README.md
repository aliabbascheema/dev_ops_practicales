# DevOps Practicals with GitHub and GitHub Actions  

This repository is a **simple Django application skeleton** designed to demonstrate **version control** and **CI/CD workflows** using GitHub and GitHub Actions. The project is a practical implementation of key DevOps principles, including automation, collaboration, and streamlined deployment.  

## Features  

- **Django Framework**:  
  A minimal Django setup to build and deploy web applications.  

- **GitHub Integration**:  
  - Version control using GitHub for collaborative development.  
  - Clear branching strategy with main, development, and feature branches.  
  - Commit history demonstrating best practices in logging changes.  

- **GitHub Actions CI/CD Pipeline**:  
  - Automated testing with Django’s test suite.  
  - Deployment workflow to a staging/production environment.  
  - Notifications for build successes or failures.  

- **DevOps Workflow Demonstration**:  
  - Continuous integration and delivery practices.  
  - Collaborative tools and strategies for efficient project management.  


## Prerequisites  

1. Python 3.8+  
2. pip and virtualenv  
3. Git  
4. A GitHub account for repository hosting and GitHub Actions configuration  

## Installation  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/aliabbascheema/dev_ops_practicales.git  
   cd dev_ops_practicales 
   ```  

2. **Set Up a Virtual Environment**:  
   ```bash  
   python -m venv venv  
   source venv/bin/activate  # On Windows: venv\Scripts\activate  
   ```  

3. **Install Dependencies**:  
   ```bash  
   pip install -r requirements.txt  
   ```  

4. **Run Initial Migrations**:  
   ```bash  
   python manage.py migrate  
   ```  

5. **Run the Development Server**:  
   ```bash  
   python manage.py runserver  
   ```  

   Access the application at `http://127.0.0.1:8000/`.

## Usage  

### Branching Strategy  

- **Main**: Stable branch for production-ready code.  
- **Development**: Active development occurs here before merging into `main`.  
- **Feature/<name>**: Isolated feature branches for specific tasks.  

### GitHub Actions Workflow  

The repository includes a pre-configured `.github/workflows/django-ci.yml` file to automate:  
1. **Linting and Testing**: Ensures code quality with automated test runs.  
2. **Build Process**: Verifies the application builds successfully.  
3. **Deployment**: Automates deployment to staging or production environments.  

## Directory Structure  

```plaintext  
dev_ops_practicales/  
├── manage.py  
├── dev_ops_practicales/  
│   ├── __init__.py  
│   ├── admin.py  
│   ├── apps.py  
│   ├── migrations/  
│   ├── models.py  
│   ├── tests.py  
│   ├── views.py  
├── templates/  
├── static/  
├── requirements.txt  
├── .github/  
│   └── workflows/  
│       └── django-ci.yml  
└── README.md  
```  

## Testing  

Run tests locally using Django’s test runner:  
```bash  
python manage.py test  
```  

## Limitations  

- The application is a skeleton and does not include business-specific logic or advanced features.  
- Deployment configuration assumes basic setups and may require customization for advanced use cases.  

## Future Enhancements  

- Add Docker for containerized deployments.  
- Integrate advanced monitoring tools like Prometheus and Grafana.  
- Expand CI/CD pipelines to include multi-environment support.  


## Contributions  

Contributions are welcome! Fork the repository, make your changes, and submit a pull request.  

## License  

This project is licensed under the MIT License. See the `LICENSE` file for more details.  
