# 180825_hw

Модуль: Системи контролю версій  
Тема: Системи контролю версій. Частина 2

# Завдання 1
 При виконуванні завдань необхідно використовувати репозиторій на GitHub. Використовуйте ваш обліковий запис на GitHub. Якщо у вас його немає, створіть.
## git config user.email && git config user.name
    potereyko@gmail.com
    Volodymyr Potereiko(AIPython52)

# Завдання 2
 Створіть папку з набором підпапок і файлів.

## $ mkdir main_folder && cd main_folder && touch file1.txt file2.txt
## $ ls -l

    total 0
    -rw-r--r-- 1 user 197121 0 Aug 24 23:30 file1.txt
    -rw-r--r-- 1 user 197121 0 Aug 24 23:30 file2.txt

# Завдання 3
Створіть репозиторій у головній папці.

# Завдання 4
Додайте весь вміст папки в індекс репозиторія за допомогою команди: git add.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/main_folder (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ../README.md                                                                                                                                                                                                    

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ./                                                                                                                                                                                                                          

no changes added to commit (use "git add" and/or "git commit -a")

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/main_folder (master)                                                                                                                                     
$ git add .

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/main_folder (master)                                                                                                                                     
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file1.txt                                                                                                                                                                                                       
        new file:   file2.txt                                                                                                                                                                                                       

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ../README.md 

# Завдання 5
Створіть commit на підставі даних, доданих в індекс. Використайте команду: git commit.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (master)
$ gh auth status
github.com
  ✓ Logged in to github.com account potervi94 (keyring)
  - Active account: true
  - Git operations protocol: https
  - Token: ghp_************************************
  - Token scopes: 'admin:enterprise', 'admin:gpg_key', 'admin:org', 'admin:org_hook', 'admin:public_key', 'admin:repo_hook', 'admin:ssh_signing_key', 'audit_log', 'codespace', 'copilot', 'delete:packages', 'gist', 'notifications', 'project', 'repo', 'user', 'workflow', 'write:discussion', 'write:network_configurations', 'write:packages'

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md                                                                                                                                                                                                       

no changes added to commit (use "git add" and/or "git commit -a")

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (master)                                                                                                                                                 
$ git commit -am "Task 5"
[master 2d4eb84] Task 5
 1 file changed, 13 insertions(+)

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (master)                                                                                                                                                 
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

# Завдання 6
Створіть нову гілку з назвою newbranch.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (master)                                                                                                                                                 
$ git switch -c newbranch
Switched to a new branch 'newbranch'

- Завдання 7: Створіть нову підпапку з набором файлів, наповніть їх даними. Після наповнення створіть commit із вмістом нової підпапки в гілці newbranch.
- Завдання 8: Перейдіть у гілку master. Створіть нову підпапку з файлами, наповніть їх даними. Після наповнення створіть commit із вмістом нової папки в гілці master.
- Завдання 9: Перейдіть у гілку newbranch. Злийте вміст гілки master з гілкою newbranch.
- Завдання 10: Перейдіть у гілку master. Внесіть зміни в кілька використаних файлів. Зміни мають привести до конфліктів при злитті. Створіть commit зі змінами.
- Завдання 11: Перейдіть у гілку newbranch. Злийте вміст гілки master з гілкою newbranch. Розв'яжіть конфлікти при їх виникненні.
