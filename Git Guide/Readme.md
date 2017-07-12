# git command line (Feat.git-scm)
``` Python
1.初始化                  >> git init

2.アプロードのリスト      >> git add .

2.リストを確認する        >> git status

2.アプロードを削除する    >> git rm .

3.坂本を新しいする        >> git commit -m "description"

4.接続する                >> git remote add <origin> <https://github.com/artmusic0/my-first.git>

5.アップロードする        >> git push -u origin master

O.坂本更新                >> git pull

O.正式VSベータ版          >> git checkout -b <newbrench>

O.開発中で変身する        >> git merge <newbrench>

O.プラジェトをコーピする  >> git clone <address.git>
```
Submodules
https://git-scm.com/book/en/v2/Git-Tools-Submodules
```
git submodule add <website.git>
```

Large file
https://git-lfs.github.com/
```
git lfs install
git lfs track "*.psd"
-------
git add file.psd
git commit -m "Add design file"
git push origin master
```
