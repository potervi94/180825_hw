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

# Завдання 7
Створіть нову підпапку з набором файлів, наповніть їх даними.
Після наповнення створіть commit із вмістом нової підпапкив гілці newbranch.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (newbranch)                                                                                                                                              
$ mkdir newbranch_folder

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw (newbranch)                                                                                                                                              
$ cd newbranch_folder

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
$ echo "### This is nebranch ####" >> newbranch_file.txt

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)
$ git add  newbranch_file.txt
warning: in the working copy of 'newbranch_folder/newbranch_file.txt', LF will be replaced by CRLF the next time Git touches it

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
$ git status
On branch newbranch
Your branch is up to date with 'origin/newbranch'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   newbranch_file.txt                                                                                                                                                                                              

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ../README.md                                                                                                                                                                                                    


user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
$ git commit -am "Task 7"
[newbranch 229f6f7] Task 7
 2 files changed, 7 insertions(+), 1 deletion(-)
 create mode 100644 newbranch_folder/newbranch_file.txt

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
### $ git status
    On branch newbranch
    Your branch is ahead of 'origin/newbranch' by 1 commit.
    (use "git push" to publish your local commits)
    
    nothing to commit, working tree clean

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
### $ git push -u origin HEAD
    Enumerating objects: 7, done.
    Counting objects: 100% (7/7), done.
    Delta compression using up to 32 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (5/5), 485 bytes | 121.00 KiB/s, done.
    Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
    remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
    To https://github.com/potervi94/180825_hw.git
    a042d46..229f6f7  HEAD -> newbranch
    branch 'newbranch' set up to track 'origin/newbranch'.

# Завдання 8
Перейдіть у гілку master. Створіть нову підпапку з файлами, наповніть їх даними. Після наповнення створіть commit із вмістом нової папки в гілці master.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (newbranch)                                                                                                                             
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (master)                                                                                                                                
$ mkdir new_master_folder

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder (master)                                                                                                                                
$ cd new_master_folder

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder/new_master_folder (master)                                                                                                              
$ echo "### This is master ####" >> master_file.txt

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder/new_master_folder (master)                                                                                                              
$ git add master_file.txt
warning: in the working copy of 'newbranch_folder/new_master_folder/master_file.txt', LF will be replaced by CRLF the next time Git touches it

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder/new_master_folder (master)                                                                                                              
$ git commit -am "Завдання 8"

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder/new_master_folder (master)                                                                                                              
$ git commit -am "Завдання 8"
[master 325708b] ╨Ч╨░╨▓╨┤╨░╨╜╨╜╤П 7(╤З╨╡╤А╨╡╨╖8
 2 files changed, 91 insertions(+), 3 deletions(-)
 create mode 100644 newbranch_folder/new_master_folder/master_file.txt

user@CEPBEPOKK MINGW64 ~/OneDrive/__AIPYTHON52/ALL_TASKS/08_2025/180825_hw/newbranch_folder/new_master_folder (master)                                                                                                              
$ git push -u origin HEAD
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 32 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (6/6), 1.40 KiB | 238.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/potervi94/180825_hw.git
   352e9e7..325708b  HEAD -> master
branch 'master' set up to track 'origin/master'.

- Завдання 9: Перейдіть у гілку newbranch. Злийте вміст гілки master з гілкою newbranch.
- Завдання 10: Перейдіть у гілку master. Внесіть зміни в кілька використаних файлів. Зміни мають привести до конфліктів при злитті. Створіть commit зі змінами.
- Завдання 11: Перейдіть у гілку newbranch. Злийте вміст гілки master з гілкою newbranch. Розв'яжіть конфлікти при їх виникненні.
