# Gym-Git-Exercise-Solutions
//BUNDLE 1
exercise 1
git init
git branch
git branch -M main
git status
git add .
git commit -m "feat: initialize project"
git remote add origin https://github.com/dojdev153/git-exercises.git
git remote -v
git push -u origin main
git switch -c dev
git switch -c test
git switch dev
git branch -d test
git branch

exercise 2
git switch dev
git stash push -u -m "home page changes"
git status
git stash push -u -m "about page changes"
git stash list
git stash push -u -m "team page changes"
git stash list
git stash pop stash@{1}
git stash list
git stash pop stash@{1}
git status
git add .
git commit -m "feat: add home and about pages"
git push -u origin dev
git stash list
git stash pop stash@{0}
git status
git reset
git clean -f

//BUNDLE2
exercise 1
git branch
git switch dev
git pull origin dev
git switch -c ft/bundle-2
git status
git add services.html
git commit -m "feat: add services page"
git log --oneline --all --decorate
git push -u origin ft/bundle-2
git switch main
git pull origin main
git branch -d ft/bundle-2

exercise 2
git branch
git switch main
git pull origin main
git switch -c ft/service-redesign
git status
git add service.html
git commit -m "feat: redesign service page"
git push -u origin ft/service-redesign
git switch main
git pull origin main
git add service.html
git commit -m "feat: update service heading"
git push origin main
git switch ft/service-redesign
git diff main
git merge main
git status
git add service.html
git commit -m "merge: resolve service page conflict"
git push origin ft/service-redesign
