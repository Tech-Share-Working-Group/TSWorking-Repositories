# 1. アプリ実行方法

## 1-1. アプリを取得

```bash
# Ubuntu/bash

cd ~
mkdir rensyu && cd rensyu
git clone --no-checkout git@github.com:Tech-Share-Working-Group/template.git .

# 特定のディレクトリのみ取得
git sparse-checkout set /01_sample/00_deliverables/b23a0253_app

# 反映
git checkout main

cd 01_sample/00_deliverables/b23a0253_app

ls
```

<details>
<summary>コンソール結果</summary>

```bash
# Ubuntu/bash

# 「ls」

```
</details>

</br>

## 1-2. Dockerを起動

```bash
# Ubuntu/bash

docker build -t xxxxx-app .
docker run -p 8080:8080 xxxxx-app
```

[http://localhost:8080/](http://localhost:8080/)にアクセス

![image](https://github.com/user-attachments/assets/5f061512-3173-49d3-a71e-60e60f727cdc)
