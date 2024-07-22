```python
class Sarah:
    def __init__(self):
        self.username = 'ssin0045'
        self.name = 'Sarah Singh'
        self.position = 'Data Engineer'
        self.interests = [
            "Data Science", "Machine Learning", "Artificial Intelligence",
            "Cloud Computing", "Big Data"
        ]
        self.location = "Sydney, Australia"
        self.education = {
            'Master of Data Science': 'Swinburne University of Technology',
            'Bachelor of Business Analytics': 'Monash University',
            'Bachelor of Commerce (Finance)': 'Monash University'
        }
        self.background = {
            'Consultant': 'Education Centre of Australia',
            'Data Analyst Intern': 'Sircel',
            'Social Media Analyst': 'AEMC'
        }
        self.skills = {
            'programming': ['Python', 'SQL', '.NET', 'Java', 'C++', 'R', 'PHP'],
            'database': ['PostgreSQL', 'MySQL', 'SQLite3', 'MongoDB', 'Redis'],
            'devops': ['Docker', 'Linux', 'GitHub Actions', 'AWS', 'Azure'],
            'frontend': ['HTML', 'CSS', 'JavaScript', 'Svelte', 'Bootstrap'],
            'tools': ['GIT', 'GitHub', 'GitLab', 'Pandas', 'Jupyter Notebook', 'SQLAlchemy', 'Celery', 'Nginx', 'R'],
            'misc': ['Firebase', 'TDD', 'SCRUM', 'SOLID', 'gRPC', 'ML', 'Tech Writing']
        }
        self.architecture = ['SPA', 'MVC', 'Serverless', 'Microservices']

    def __str__(self):
        return f'{self.name} | {self.position}'

if __name__ == '__main__':
    sarah = Sarah()
    print(sarah)
