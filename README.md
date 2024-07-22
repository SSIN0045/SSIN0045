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

    def display_info(self):
        print(f"Username: {self.username}")
        print(f"Name: {self.name}")
        print(f"Position: {self.position}")
        print(f"Location: {self.location}")
        print("\nInterests:")
        for interest in self.interests:
            print(f"- {interest}")
        print("\nEducation:")
        for degree, institution in self.education.items():
            print(f"- {degree}: {institution}")
        print("\nBackground:")
        for role, company in self.background.items():
            print(f"- {role}: {company}")
        print("\nSkills:")
        for category, skills in self.skills.items():
            print(f"{category.capitalize()}: {', '.join(skills)}")
        print("\nArchitecture Styles:")
        for style in self.architecture:
            print(f"- {style}")

    def __str__(self):
        return f'{self.name} | {self.position}'

    def display_summary(self):
        summary = f"""
        ## {self.name} | {self.position}

        **Location:** {self.location}

        ### Interests
        {" | ".join(self.interests)}

        ### Education
        {" | ".join([f"{degree} ({institution})" for degree, institution in self.education.items()])}

        ### Background
        {" | ".join([f"{role} at {company}" for role, company in self.background.items()])}

        ### Skills
        **Programming:** {", ".join(self.skills['programming'])}
        **Database:** {", ".join(self.skills['database'])}
        **DevOps:** {", ".join(self.skills['devops'])}
        **Frontend:** {", ".join(self.skills['frontend'])}
        **Tools:** {", ".join(self.skills['tools'])}
        **Miscellaneous:** {", ".join(self.skills['misc'])}

        ### Architecture Styles
        {" | ".join(self.architecture)}
        """
        return summary

if __name__ == '__main__':
    sarah = Sarah()
    print(sarah)
    sarah.display_info()
    print("\nGitHub Markdown Summary:\n")
    print(sarah.display_summary())
