# aws ディレクトリの説明

- `./aws` は、 コンテナ内の /root/.aws として扱うためのディレクトリです
- AWSに関する credentials ,config ファイルを置くと、コンテナ起動でマウントされます
- Windowsでは、 `%USERPROFILE%\.aws`  にあるファイルの中身を置く
```
イメージとしては、以下を実施しておく
cp `%USERPROFILE%\.aws`  ./aws/
```

