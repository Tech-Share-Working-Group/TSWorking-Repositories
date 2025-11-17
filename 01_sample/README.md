# 1. 作成者について
| id | 作成日 | 一言コメント |
| ---- | ---- | ---- |
| [b23a0253](https://github.com/TSWG-b23a0253) | 2025/06/29 |  |

</br></br>

# 2. こちらのディレクトリについて
こちらではXXXXXの構築手順を説明いたします。

</br></br>

# 3. 必要な環境

- [Practice-WSL](https://github.com/Tech-Share-Working-Group/Practice-WSL/tree/main/01_Install_WSL)
- [Practice-Docker](https://github.com/Tech-Share-Working-Group/Practice-Docker/tree/main/01_Install_Docker)
- [Practice-Git](https://github.com/Tech-Share-Working-Group/Practice-Git/tree/main/01_Install_Git)
- [Install-vim](https://github.com/Tech-Share-Working-Group/Practice-Editor/tree/main/04_Use_Vim)

</br></br>

# 4. XXXXXの環境構築

## 4-1. ワークスペースの作成

[成果物フォルダ](https://github.com/Tech-Share-Working-Group/XXXXX/tree/main/XXXXX/00_deliverables)に自分のワークスペースを作成

</br>

## 4-2. ローカルに落とし、自分の作業ディレクトリに移動

```bash
# Ubuntu/bash

git clone git@github.com:Tech-Share-Working-Group/XXXXX.git

# 自分の作業ディレクトリに移動
cd Practice-Go-FrameWork/XXXXX/00_deliverables/[自分の作業ディレクトリ]/

# 作業前に pull してリモートと同期
git pull origin main --rebase
```

</br>

## 4-3. 「Dockerfile」ファイルの作成

```bash
# Ubuntu/bash

vim Dockerfile
```

<details>
<summary>「Dockerfile」のファイルの内容</summary>

```Dockerfile
# Dockerfile


```
</details>

</br></br>

# 5. 「Hello World」を表示させる

## 5-1. ビルドする

```bash
# Ubuntu/bash

docker build -t my-app .
```

<details>
<summary>コマンド結果</summary>

```bash
# Ubuntu/bash


```
</details>

</br>

## 5-2. 実行する

```bash
# Ubuntu/bash

docker run -p 8080:8080 my-app
```

<details>
<summary>コマンド結果</summary>

```bash
# Ubuntu/bash


```
</details>

</br>

## 5-3. 画面で確認

[http://localhost:8080/](http://localhost:8080/)にアクセスする。

![image](https://github.com/user-attachments/assets/b4376f3d-ec55-4dbd-a95c-cd60157f49ae)

</br></br>

# 6. githubにpushする

```bash
# Ubuntu/bash

# 「.git」フォルダがあるディレクトリまで移動
cd ../../..
ls -a

# 上記で「.gitignore」がなければ下記を実行
echo '*:[Zz]one.Identifier' >> .gitignore

# ステージ
git add . && git diff --cached --name-only

# 「git add .」で変更対象以外があれば、変更を元に戻す
git restore ファイル名

# コミットメッセージ設定
git commit -m "b23a0253 edit"

# リモートと同期して、再度上記を実行
git pull origin main --rebase

# githubにpushする
git push origin main
```

</br></nr>
