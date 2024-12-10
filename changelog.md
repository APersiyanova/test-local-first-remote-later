(в скобках мои комментарии к командам)

git init
git remote add origin git@github.com:APersiyanova/test-local-first-remote-later.git (подключиться)
git push --set-upstream origin main (первый раз) (git push -u origin main)

----
git checkout -b '1-some-issue' (создаете новую ветку и переключаетесь на неё)
git branch '1-some-issue' (создаете новую ветку, но не переключаетесь на неё)
         -u
git push --set-upstream origin 1-some-issue (первый раз)
----
git push origin main (отправить изменения в удаленный репозиторий из локального проекта)
git push origin 1-some-issue (отправить изменения в удаленный репозиторий из ветки)
----
git remote show origin

---- 
git checkout main (вернуться в main)
git status

----
(только посмотреть)
git remote show origin
git fetch
git log (git log origin/1-some-issue) (git log origin/1-some-issue ^1-some-issue)
git diff e4e772eeea7adaa2250dd85ba1d4b690a82c1dfd (указывается хэш коммита)
git show e4e772eeea7adaa2250dd85ba1d4b690a82c1dfd
----
(влить изменения на git в локальную ветку)
git pull (git pull origin 1-some-issue)
----
git remote add vendor git@github.com:APersiyanova/test-remote-is-local-no.git (подключаем локальный проект еще к одному удаленному репозиторию)
(информация о путях к удаленным репозиториям)
git remote -v
---- 
(можно удалить связь с репозиторием
git remote remove origin
git remote add origin путь
git remote set-url origin путь
git remote set-url --push origin путь)
----
