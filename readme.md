tese vi
curso git

criado para user marciaalves
email alves..
subpasta dartup


Marcia@NOT-TESTES MINGW64 ~
$ git config --global user.nome "Marcia Alves"

Marcia@NOT-TESTES MINGW64 ~
$ git config user nome
fatal: not in a git directory

Marcia@NOT-TESTES MINGW64 ~
$ git config user
error: key does not contain a section: user

Marcia@NOT-TESTES MINGW64 ~
$ config --global user.nome "marcia alves"
bash: config: command not found

Marcia@NOT-TESTES MINGW64 ~
$ git config --global user.nome "marcia alves"

Marcia@NOT-TESTES MINGW64 ~
$ git config --global user.email "enupprog@gmail.com"

Marcia@NOT-TESTES MINGW64 ~
$ git config --global core.editor sub

Marcia@NOT-TESTES MINGW64 ~
$ ls git
ls: cannot access 'git': No such file or directory

Marcia@NOT-TESTES MINGW64 ~
$ git config user.name

Marcia@NOT-TESTES MINGW64 ~
$ git config user.email
enupprog@gmail.com

Marcia@NOT-TESTES MINGW64 ~
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
credential.helper=manager
user.nome=marcia alves
user.email=enupprog@gmail.com
core.editor=sub

Marcia@NOT-TESTES MINGW64 ~
$ mkdir git course

Marcia@NOT-TESTES MINGW64 ~
$ cd git-course
bash: cd: git-course: No such file or directory

Marcia@NOT-TESTES MINGW64 ~
$ mkdir git-course

Marcia@NOT-TESTES MINGW64 ~
$ cd git-course

Marcia@NOT-TESTES MINGW64 ~/git-course
$ git init
Initialized empty Git repository in C:/Users/Marcia/git-course/.git/

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ ls -la
total 28
drwxr-xr-x 1 Marcia 197121 0 dez 24 11:08 ./
drwxr-xr-x 1 Marcia 197121 0 dez 24 11:07 ../
drwxr-xr-x 1 Marcia 197121 0 dez 24 11:08 .git/

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ cd .git/

Marcia@NOT-TESTES MINGW64 ~/git-course/.git (GIT_DIR!)
$ ls
config  description  HEAD  hooks/  info/  objects/  refs/

Marcia@NOT-TESTES MINGW64 ~/git-course/.git (GIT_DIR!)
$ cd ..

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ ls
readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ ls
readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git add readme.md
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git add readme.md
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit -m "add readme.md"
[master (root-commit) 277ef17] add readme.md
 1 file changed, 4 insertions(+)
 create mode 100644 readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit -m"vai dar erro"
On branch master
Changes not staged for commit:
        modified:   readme.md

no changes added to commit

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git add readme.md
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit -m "add link to more info"
[master c4d14b7] add link to more info
 1 file changed, 1 insertion(+), 1 deletion(-)

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ ^C

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log
commit c4d14b7976adf386ea4c92b759e0da8746f5955e (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log --decorate
commit c4d14b7976adf386ea4c92b759e0da8746f5955e (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log --author="marcia"

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git shortlog
Marcia (2):
      add readme.md
      add link to more info


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log --author="Marcia"
commit c4d14b7976adf386ea4c92b759e0da8746f5955e (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git shortlog
Marcia (2):
      add readme.md
      add link to more info


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git shortlog -sn
     2  Marcia

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log --graph
* commit c4d14b7976adf386ea4c92b759e0da8746f5955e (HEAD -> master)
| Author: Marcia <enupprog@gmail.com>
| Date:   Tue Dec 24 11:25:25 2019 -0300
|
|     add link to more info
|
* commit 277ef173a88b15abca87077b097e48e32ba28eec
  Author: Marcia <enupprog@gmail.com>
  Date:   Tue Dec 24 11:21:16 2019 -0300

      add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log
commit c4d14b7976adf386ea4c92b759e0da8746f5955e (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ ^C

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git show ^C

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git show 277ef173a88b15abca87077b097e48e32ba28eec
commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

diff --git a/readme.md b/readme.md
new file mode 100644
index 0000000..21e5287
--- /dev/null
+++ b/readme.md
@@ -0,0 +1,4 @@
+#Github
+Arquivo da aulta de Git e Github para iniciantes.
+este é um repositorio teste para ensinar como funciona:wq
+

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git dif
git: 'dif' is not a git command. See 'git --help'.

The most similar commands are
        diff
        config
        difftool
        init

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git diff
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory
diff --git a/readme.md b/readme.md
index 9098085..f431942 100644
--- a/readme.md
+++ b/readme.md
@@ -1,4 +1,6 @@
 #Github
 Arquivo da aulta de Git e Github para iniciantes.
 este é um repositorio teste para ensinar como funciona:wq
-saiba mais em [....]
+saiba mais em [....
+gostou do curso? Quer mais? Ajude com uma doação. Até um café vale.
+]

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git diff --nome-only
error: invalid option: --nome-only

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git diff -nome-only
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory
diff --git a/readme.md b/readme.md
index 9098085..1b18e13 100644
--- a/readme.md
+++ b/readme.md
@@ -1,4 +1,7 @@
 #Github
 Arquivo da aulta de Git e Github para iniciantes.
 este é um repositorio teste para ensinar como funciona:wq
-saiba mais em [....]
+saiba mais em [....
+gostou do curso? Quer mais? Ajude com uma doação. Até um café vale.
+use sempre o git diff antes de comitar
+]

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit --name-only
error: unknown option `name-only'
usage: git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup <commit>      use autosquash formatted message to fixup specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C/-c/--amend)
    -s, --signoff         add Signed-off-by:
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <mode>      how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --ahead-behind        compute full ahead/behind values
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit --name-only
error: unknown option `name-only'
usage: git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup <commit>      use autosquash formatted message to fixup specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C/-c/--amend)
    -s, --signoff         add Signed-off-by:
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <mode>      how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --ahead-behind        compute full ahead/behind values
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)


Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit -am"edit readme"
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory
[master 60a028f] edit readme
 1 file changed, 4 insertions(+), 1 deletion(-)

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log
commit 60a028fd613757e987177fc6339cfb657147d7da (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:38:13 2019 -0300

    edit readme

commit c4d14b7976adf386ea4c92b759e0da8746f5955e
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git show
commit 60a028fd613757e987177fc6339cfb657147d7da (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:38:13 2019 -0300

    edit readme

diff --git a/readme.md b/readme.md
index 9098085..1b18e13 100644
--- a/readme.md
+++ b/readme.md
@@ -1,4 +1,7 @@
 #Github
 Arquivo da aulta de Git e Github para iniciantes.
 este é um repositorio teste para ensinar como funciona:wq
-saiba mais em [....]
+saiba mais em [....
+gostou do curso? Quer mais? Ajude com uma doação. Até um café vale.
+use sempre o git diff antes de comitar
+]

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log
commit 60a028fd613757e987177fc6339cfb657147d7da (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:38:13 2019 -0300

    edit readme

commit c4d14b7976adf386ea4c92b759e0da8746f5955e
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md
i
Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git checkout readme.md
Updated 0 paths from the index

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git diff

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git reset HEAD readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git diff

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git checkout readme.md
Updated 0 paths from the index

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vim readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit -am "comittando"
warning: LF will be replaced by CRLF in readme.md.
The file will have its original line endings in your working directory
[master f0d76f3] comittando
 1 file changed, 1 insertion(+), 1 deletion(-)

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ vi readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git reset  --soft

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git log
commit f0d76f3c0fd62e6edd2fd6b75aa965e52d8399f6 (HEAD -> master)
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:43:32 2019 -0300

    comittando

commit 60a028fd613757e987177fc6339cfb657147d7da
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:38:13 2019 -0300

    edit readme

commit c4d14b7976adf386ea4c92b759e0da8746f5955e
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:25:25 2019 -0300

    add link to more info

commit 277ef173a88b15abca87077b097e48e32ba28eec
Author: Marcia <enupprog@gmail.com>
Date:   Tue Dec 24 11:21:16 2019 -0300

    add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git commit add readme.md "commit"
error: pathspec 'add' did not match any file(s) known to git
error: pathspec 'commit' did not match any file(s) known to git

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git comitt
git: 'comitt' is not a git command. See 'git --help'.

The most similar command is
        commit

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git comitt readme.md
git: 'comitt' is not a git command. See 'git --help'.

The most similar command is
        commit

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git add readme.md

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Marcia@NOT-TESTES MINGW64 ~/git-course (master)
$

teste do cursos e comandos do curso.
