1. Go to Your Project Folder
Open terminal and move to the project directory.

        for example in visual studio code (VS CODE)
        ![Folder screenshot](images/Screenshot%202026-03-12%20at%2012.23.41.png)
        

code:
            cd path/to/your/project
            cd Desktop/my-python-project

2. Initialize Git
Create a Git repository in the folder.

code:

                git init


3. Create a .gitignore File
This file tells Git what not to upload.

                touch .gitignore

    Open it and add:

    .venv/
    __pycache__/
    *.pyc
    .env
    .DS_Store

4. Add Files to Git

        git add .

        Because .venv is in .gitignore, it will not be staged.


5. Commit the Files

        git commit -m "Initial project commit"

6. Create a Repository on GitHub
        Go to GitHub
        Click New Repository
        Give it a name
        Do NOT initialize with README (since you already have files)
        Example repo:

        my-python-project

7. Connect Local Repo to GitHub
GitHub will give a command like this. Run it in your terminal

code:

    git remote add origin https://github.com/username/repository-name.git

    for example:
    git remote add origin https://github.com/tonynyamao/docker-vuln-project.git


8. Push the Project to GitHub

code:
            git branch -M main
            git push -u origin main

9. Confirm .venv is Ignored

code:

            git status

            .venv should not appear in the staged files.

    