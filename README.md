## Setting Up the Repository and Development Branch

Follow these steps to set up a new GitHub repository and create a development branch:

1. **Create a local directory for the project:**
   ```bash
   mkdir new-project
   cd new-project
   ```

2. **Initialize a new Git repository:**
   ```bash
   git init
   ```

3. **Create the initial README.md file:**
   ```bash
   echo "# New Project" > README.md
   git add README.md
   git commit -m "init"
   ```

4. **Create and switch to the development branch:**
   ```bash
   git checkout -b development
   ```

5. **Add detailed instructions to README.md and commit them:**
   - Edit `README.md` and include these setup steps.
   - Then commit:
     ```bash
     git add README.md
     git commit -m "PROM-42164 #comment Add setup instructions to README.md"
     ```

6. **Push the repository to GitHub:**
   ```bash
   git remote add origin <your-repository-URL>
   git push -u origin development
   ```

7. **Create a pull request or merge development to main once verified:**
   ```bash
   git checkout main
   git merge development
   git push origin main
   ```
