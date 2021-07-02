# ssh ディレクトリの説明

- `./ssh` は、 コンテナ内の /root/.ssh として扱うためのディレクトリです
- コンテナ内からGitリポジトリにssh key接続する場合の 公開鍵と秘密鍵を置く
- Windowsでは、 `%USERPROFILE%\.ssh`  にあるファイルの中身を置く
```
イメージとしては、以下を実施しておくが、ssh鍵のフォーマットが違う場合はコピーしても Githubには invalid で接続できない。
cp `%USERPROFILE%\.ssh`  ./ssh/
```
- Windows と Mac/Linux では保存される公開鍵のフォーマットが違う。そのためwindowsでは、PuTTY key で生成した場合は、OpenSSH2フォーマットに変える必要がある

