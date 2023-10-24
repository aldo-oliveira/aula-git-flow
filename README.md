# aula-git-flow
https://www.youtube.com/watch?v=dJjVr6Ya7B8&t=1819s

ggit flow - delivery flow

# 1) start config git flow
branch 'main': (production)
git flow init (start config and branches definition)
create branches structure
main - production
develop - dev
feature branch - demanda
release branch - version/tag to production
hotfix - ajustes

# 2) create features based on develop
branch 'develop': (development)
git flow feature start 12345
- created new branch feature/12345
- checkout new branch feature/12345

git flow feature publish 12345  obs: publish/push to others devs

git flow feature finish 12345 obs: finish
- update branch based on develop
- delete branch feature/12345
- checkout 'develop'

# 3) release to production
branch 'develop':
git flow release start 1.0
- created based on develop
- checkout 'release/1.0

git flow release finish '1.0'
- merge into main
- cria tag 1.0
- merge into develop
- delete release/1.0
- checkout develop

# 4) hotfix
git flow hotfix start my_hotfix
- new branch based on 'main'
- checkout branch hotfix/my_hotfix

git flow hotfix finished my_hotfix
- hotfix merged into 'main'
- hotfix merged into 'develop'
- deleted hotfix branch
- checkout develop

git push --all
-publish all changes