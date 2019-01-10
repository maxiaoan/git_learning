  434  cd git_learning/
  438  ls
  442  mkdir  images 
  443  mv git-logo.png  images/
  445  rm README.md 
  447  rm -r git_learning/
  451  git status 
  453  ls -al
  454  git status 
  455  git add index.html images/ styles/ js/
  456  git status 
  459  git commit  -m'add index and logo'
  460  git add readme 
  461  git status 
  462   git commit -m 'add readme'
  463  git status 
  464  git log 
  475  git status 
  476  git add -u
  478  git status 
  479  git commit -m'add reference project'
  480  git log 
  483  mv readme readme.md
  484  git status 
  486   git rm  readme
  489  git status 
  490  git log 
  492  git mv readme readme.md
  493  git status 
  495  history 
  496  git commit -m'rename  readme to readme.md'
  497  git status 
  498  git log 
  500  git log --oneline 
  501   git push  origin  master 
  502  cat readme.md 
  503  vim readme.md 
  505  git status 
  506  git add -u
  507  git commit  -a
  509  git status 
  510  git push  origin  master 
  511  git add readme.md
  512  git status 
  513  git commit  -m'modified readme.md'
  514  git status 
  515  git push  origin  master 
  516  git log -n 2
  517  git log -n 2 --oneline 
  518  git branch -v
  519  git branch -va
  520  git log --oneline --all
  521  git log --oneline --all -n4 --graph 
