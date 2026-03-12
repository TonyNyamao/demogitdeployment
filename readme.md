1. Go to Your Project Folder
Open terminal and move to the project directory.

        Exampkle of project folder in visual studio code (VS CODE)

<img src="images/Screenshot 2026-03-12 at 12.23.41.png" width="300">
        

example of how the terminal can look like:

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
        step 1 : Go to GitHub

        step 2: Click New Repository

        step 3: Give it a name

        **Do NOT initialize with README (since you already have files)**

        Example repository name:

                  my-python-project

7. Connect Local Repo to GitHub
GitHub will give a command like this. Run it in your terminal

After the add (statement below) replace the link with your repository link by copying the link of the browser tab.

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

    