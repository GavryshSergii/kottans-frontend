- git diff
- git log
- git add
- git commit
- git commit --amend


- git checkout nameBranch
- git checkout hasheBransh
- git branch newBranch
- git checkout -b newBranch - create a new branch and switch to it
- git merge someBranch
- git rebase someBranch - moves the current branch after the specified
- git checkout someBranch^ - go to the first parent of someBranch
- git checkout someBranch~2 - go to the second parent of someBranch
- git branch -f whatPointer wherePut
- git branch -f main HEAD~2 - moves main to second parent HEAD 

git reset HEAD~1
git revert HEAD

- git cherry-pick [[commit1] commit2]
- git cherry-pick C2 C4 - додасть до поточної гілки перелічені комміти
- git rebase -i someCommit - надасть можливість переглянути поточну гілку до зазначеного комміту (порядок, перелік коммітів, а також може об'єднати деякі)

git tag v1 branch



Git describe має наступну форму:

git describe <посилання>

Де <посилання> -- це будь-що, що вказує на конкретний коміт. Якщо ти не вкажеш посилання, git використає поточну локацію (HEAD).

Вивід команди виглядає як:

<таг>_<к-ть комітів>_g<хеш>

де таг -- це найближчий попередній таг з історії; к-ть комітів -- це наскільки далеко цей таг в історії, а <хеш> -- це хеш коміту, який описується.


Так само як і модифікатор ~, модифікатор ^ також приймає необов’язкове число після нього.

Замість того, щоб вказувати кількість генерацій щоб переміститись назад (те що робить ~), число після ^ вказує на яке батьківське посилання мерджу потрібно перейти. Зауважте що так як мерджевий коміт має декілька батьків, використання '^' без числа є неоднозначним.

Git зазвичай перейде на "першого" з батьків вверх з мерджевого коміту, але вказання числа після ^ змінює цю поведінку.
 
 


$ git rebase -i main caption
$ git commit --amend
$ git rebase -i main caption
$ git rebase caption main

$ git checkout main
$ git cherry-pick C2
$ git commit --amend
$ git cherry-pick c3

// рішення розбіжностей в історії
// варіант 1 rebase
$ git fetch;
$ git rebase o/main;
$ git push;

//варіант 2 merge
$ git fetch;
$ git merge o/main;
$ git push;

//варіант 3 rebase
$ git pull --rebase;
$ git push;
 
//варіант 4 merge
$ git pull;
$ git push;


fakeTeamwork - симуляція колективної роботи у застосунку

