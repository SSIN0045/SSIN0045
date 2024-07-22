class sarah:
 def __init__(self):
        self.username = 'ssin0045'
        self.name = 'Sarah Singh'
        self.position = 'Data Engineer'
        self.interest = "Data Science, Machine Learning, Artificial Intelligence, Cloud Computing, Big Data"
        self.location = "Sydney, Australia"
        self.education = {
            'Master of Data Science: Swinburne Univeristy of Technology',
            'Bachelor of Business Analytic: Monash University',
            'Bachelor of Commerce (Finance): Monash University'
        }
        self.background {
            'Consultant: Education Centre of Australia',
            'Data Analayst Intern: Sircel',
            'Social Media Analyst: AEMC',  
        } 
        self.code = {
            'programming': ['Python', 'SQL', '.NET', 'Java', 'C++', 'R', 'PHP'],
            'database': ['PostgreSQL', 'MySQL', 'SQLite3', 'Mongo DB', 'Redis'],
            'devops': ['Docker', 'Linux', 'GitHub Actions', 'AWS', 'Azure'],
            'frontend': ['HTML', 'CSS', 'JavaScript', 'Svelte', 'Boostrap'],
            'tools': ['GIT', 'GitHub', 'GitLab', 'Pandas', 'Jupyter notebook', 'SQLAlchemy', 'Celery', 'Nginx', R],
            'misc': ['Firebase', 'TDD', 'SCRUM', 'SOLID', 'gRPC', 'ML', 'Tech Writer']
        }
        self.architecture = ['SPA', 'MVC', 'Serverless', 'microservices']

    def __str__(self):
        return f'{self.name} | {self.position}'


if __name__ == '__main__':
    me = RafnixG()
    print(me)
