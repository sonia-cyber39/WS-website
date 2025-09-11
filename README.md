White Stone Test Project

Welcome to the White Stone Test Project repository! This project contains the files and assets for the White Stone website, including HTML, CSS, images, and documentation.

📁 Repository Structure
/image          → All images used on the website
/styles.css     → Main CSS file for styling
/index.html     → Main HTML file
/user-guide/    → Documentation and workflow instructions
.vscode/        → VS Code editor settings
.git/           → Git repository metadata

🌿 Branches

main → Stable version of the website. Only merge reviewed code here.

featureproperties/image → Feature branch for property section development and adding/updating images.

💡 Always use a feature branch for new work to keep main stable.

📝 user-guide Folder

The user-guide folder contains instructions and documentation for developers.
Currently, it includes:

README.md → This file, which explains Git workflow, branch usage, and project structure.

⚡ Recommended Git Workflow

1️⃣ Check Current Branch
git status       # See if working tree is clean
git branch       # Check current branch
git checkout main  # Switch to main branch if needed

2️⃣ Add New Files or Folders
git add user-guide/  # Stage the folder
# OR add all changes at once
git add .

3️⃣ Commit Changes
git commit -m "Add user-guide folder with README.md"

4️⃣ Switch to Feature Branch
git checkout featureproperties/image

5️⃣ Work on Features

Edit index.html, styles.css, or add images in /image.

Commit changes regularly in the feature branch:

git add index.html
git commit -m "Add/update property cards in properties section"

6️⃣ Review Changes
git diff main..featureproperties/image


See what has changed compared to the main branch.

7️⃣ Merge Back to Main
git checkout main
git merge featureproperties/image

8️⃣ Push Branch to GitHub (Optional)
git push origin featureproperties/image


Other team members can create a Pull Request for review before merging.

✅ Best Practices

Always work in a feature branch.

Commit frequently with meaningful messages.

Keep the main branch clean and stable.

Use user-guide for notes, instructions, or documentation.

Review changes before merging to avoid breaking the main branch.

👨‍💻 Team Member Instructions

Clone the repository or pull the latest changes.

Switch to the featureproperties/image branch to work on the property section.

Edit index.html and styles.css or add images to /image.

Stage and commit your changes:

git add .
git commit -m "Add new property cards"


Push your branch and create a Pull Request for review.

📌 Tips

Keep commits small and descriptive.

Use feature branches for experimental work.

Always check git status before switching branches.

Review git diff to see changes before merging.

This README ensures that any developer joining the project can quickly understand the repo structure, workflow, and best practices.
