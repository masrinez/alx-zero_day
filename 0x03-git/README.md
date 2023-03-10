Testing out this feature for the first time
oot@83ca6f59fc2b:/# pwd
/
root@83ca6f59fc2b:/# ls
0x02_emacs      alx-zero_day  bin   c    etc   js   lib32  libx32   media  opt   root  sbin  sys  usr
alx-pre_course  bash          boot  dev  home  lib  lib64  main.py  mnt    proc  run   srv   tmp  var
root@83ca6f59fc2b:/# cd alx-zero_day
root@83ca6f59fc2b:/alx-zero_day# ls
root@83ca6f59fc2b:/alx-zero_day# ls -l
total 0
root@83ca6f59fc2b:/alx-zero_day#  mkdir 0x03-git
root@83ca6f59fc2b:/alx-zero_day# ls
0x03-git
root@83ca6f59fc2b:/alx-zero_day# cd 0x03-git
root@83ca6f59fc2b:/alx-zero_day/0x03-git# touch README.md
root@83ca6f59fc2b:/alx-zero_day/0x03-git# echo "# 0x03-git" > README.md
root@83ca6f59fc2b:/alx-zero_day/0x03-git# 
root@83ca6f59fc2b:/alx-zero_day/0x03-git# This is a README.md file in the 0x03-git directory.
bash: This: command not found
root@83ca6f59fc2b:/alx-zero_day/0x03-git# echo "# 0x03-git" > README.md
root@83ca6f59fc2b:/alx-zero_day/0x03-git# 
root@83ca6f59fc2b:/alx-zero_day/0x03-git# This is a README.md file in the 0x03-git directory.
bash: This: command not found
root@83ca6f59fc2b:/alx-zero_day/0x03-git# pwd
/alx-zero_day/0x03-git
root@83ca6f59fc2b:/alx-zero_day/0x03-git# ls
README.md
root@83ca6f59fc2b:/alx-zero_day/0x03-git# echo "This is a README.md file in the 0x03-git directory" > README.md
root@83ca6f59fc2b:/alx-zero_day/0x03-git# cd ..
root@83ca6f59fc2b:/alx-zero_day# touch README.md
root@83ca6f59fc2b:/alx-zero_day# echo "This is a README.md file in the root directory of the alx-zero_day repository" > README.md
root@83ca6f59fc2b:/alx-zero_day# git add .
root@83ca6f59fc2b:/alx-zero_day# git commit -m "Add 0x03-git directory and README.md files" 
[master (root-commit) ac2bde1] Add 0x03-git directory and README.md files
 2 files changed, 2 insertions(+)
 create mode 100644 0x03-git/README.md
 create mode 100644 README.md
root@83ca6f59fc2b:/alx-zero_day# git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://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@github.com/masrinez/alx-zero_day.git'
root@83ca6f59fc2b:/alx-zero_day# git push origin master
Password for 'https://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@github.com': 
To https://github.com/masrinez/alx-zero_day.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://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@github.com/masrinez/alx-zero_day.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
root@83ca6f59fc2b:/alx-zero_day# git push --help
root@83ca6f59fc2b:/alx-zero_day# git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

root@83ca6f59fc2b:/alx-zero_day# git push --set -upstream origin master
error: unknown switch `p'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --recurse-submodules[=(check|on-demand|no)]
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=(yes|no|if-asked)]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

root@83ca6f59fc2b:/alx-zero_day# git push repo
fatal: 'repo' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
root@83ca6f59fc2b:/alx-zero_day# git push origin master
Password for 'https://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@github.com': 
To https://github.com/masrinez/alx-zero_day.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://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@github.com/masrinez/alx-zero_day.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
root@83ca6f59fc2b:/alx-zero_day# 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g
bash: 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g: command not found
root@83ca6f59fc2b:/alx-zero_day# git fetch origin
warning: no common commits
remote: Enumerating objects: 50, done.
remote: Counting objects: 100% (50/50), done.
remote: Compressing objects: 100% (30/30), done.
remote: Total 50 (delta 7), reused 50 (delta 7), pack-reused 0
Unpacking objects: 100% (50/50), 4.87 KiB | 48.00 KiB/s, done.
From https://github.com/masrinez/alx-zero_day
 * branch            HEAD       -> FETCH_HEAD
root@83ca6f59fc2b:/alx-zero_day# git merge master
Already up to date.
root@83ca6f59fc2b:/alx-zero_day# git push origin master
Password for 'https://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@github.com': 
To https://github.com/masrinez/alx-zero_day.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://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@github.com/masrinez/alx-zero_day.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
root@83ca6f59fc2b:/alx-zero_day# git fetch origin
From https://github.com/masrinez/alx-zero_day
 * branch            HEAD       -> FETCH_HEAD
root@83ca6f59fc2b:/alx-zero_day# git checkout master
Already on 'master'
root@83ca6f59fc2b:/alx-zero_day# git merge origin/master
merge: origin/master - not something we can merge
root@83ca6f59fc2b:/alx-zero_day# git push origin master
Password for 'https://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@github.com': 
To https://github.com/masrinez/alx-zero_day.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://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@github.com/masrinez/alx-zero_day.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
