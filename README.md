📘 Git Assignment Submission
This document provides answers to commonly encountered Git scenarios, demonstrating practical command-line usage for version control, collaboration, and workflow management.

📄 Contents
Staging and Committing Changes

Moving Commits to the Correct Branch

Creating a New Branch and Pushing to Remote

Contributing to Open-Source Projects

Resolving Merge Conflicts

Creating Feature Branches from Main

Reverting to a Specific Commit

Restoring a Deleted File

✅ 1. Staging and Committing Changes
To stage and commit all changes in your working directory:

bash
Copy
Edit
git add .
git commit -m "Your meaningful commit message here"
🔄 2. Moving Commits to the Correct Branch
If you committed to the wrong branch:

bash
Copy
Edit
git checkout -b temp-branch
git checkout correct-branch
git merge temp-branch
git branch -d temp-branch
🌿 3. Creating a New Branch and Pushing to Remote
bash
Copy
Edit
git checkout -b feature-branch
git add .
git commit -m "Add feature implementation"
git push -u origin feature-branch
🤝 4. Contributing to Open-Source Projects
Fork the repository on GitHub

Clone it:

bash
Copy
Edit
git clone https://github.com/your-username/project-name.git
cd project-name
Create a new branch:

bash
Copy
Edit
git checkout -b fix-bug-or-add-feature
Make changes, then commit:

bash
Copy
Edit
git add .
git commit -m "Describe your changes"
Push the branch:

bash
Copy
Edit
git push origin fix-bug-or-add-feature
Open a Pull Request on GitHub

⚔️ 5. Resolving Merge Conflicts
bash
Copy
Edit
git checkout your-branch
git merge main
# Resolve conflicts manually
git add .
git commit
🧪 6. Creating Feature Branches from Main
bash
Copy
Edit
git checkout main
git pull origin main
git checkout -b feature-branch
⏪ 7. Reverting to a Specific Commit
bash
Copy
Edit
git reset --hard <commit-hash>
⚠️ This will permanently remove all commits after the specified hash.

♻️ 8. Restoring a Deleted File
bash
Copy
Edit
git checkout HEAD^ -- path/to/deleted-file
git add path/to/deleted-file
git commit -m "Restore accidentally deleted file"
📌 Notes
All Git commands were tested in a Unix-based terminal.

Commands are suitable for general use, but always make a backup when using destructive operations like reset --hard.
