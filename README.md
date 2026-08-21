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

//BUNDLE 3
exercise 1
git switch main
git pull origin main
git switch -c ft/team-page
git add team.html
git commit -m "feat: add team page"
git push -u origin ft/team-page
git switch main
git pull origin main
git switch -c ft/contact-page
git switch ft/team-page
git log --oneline
git switch ft/contact-page
git cherry-pick <TEAM_COMMIT_HASH>
git add contact.html
git commit -m "feat: add contact page"
git push -u origin ft/contact-page
git switch -c ft/faq-page
git add faq.html
git commit -m "feat: add faq page"
git push -u origin ft/faq-page
git revert <TEAM_COMMIT_HASH>
git push

exercise 2
git switch ft/faq-page
git switch -c ft/home-page-redesign
git branch
git switch main
git add .
git commit -m "feat: update main branch"
git push origin main
git switch ft/home-page-redesign
git rebase main
git status
git add .
git rebase --continue
git rebase --abort
git add home.html
git commit -m "feat: redesign home page"
git push -u origin ft/home-page-redesign

//BUNDLE 4
exercise 1
git switch main
git branch
git pull origin main
git remote add git-copy https://github.com/dojdev153/git-exercise-copy.git
git remote -v
git add home.html
git commit -m "feat: update home page"
git push origin main
git push -u git-copy main
git branch -r

exercise 2
git switch main
git pull origin main
git switch -c ft/footer
git add .
git commit -m "feat: add footer"
git add .
git commit -m "feat: update footer"
git push -u origin ft/footer
git switch main
git pull origin main
git switch -c ft/squashing
git merge --squash ft/footer
git status
git commit -m "footer changes squashing"
git push -u origin ft/squashing

//BUNDLE 5
exercise 2
git clone https://github.com/YOUR-USERNAME/git-cafe-exercise.git
cd git-cafe-exercise
git remote -v
git switch -c ft/restaurant-text
git status
git diff
git add index.html
git commit -m "fix: update restaurant welcome text"
git push -u origin ft/restaurant-text

//BUNDLE 6
exercise 1
