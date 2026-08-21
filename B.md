# 手順

## 手順1
GitGub上にリモートリポジトリを用意
<img width="1672" height="458" alt="スクリーンショット 2026-08-21 145427" src="https://github.com/user-attachments/assets/c5443749-f7bb-4cf0-a8d2-e33244f10d59" />
cloneしローカルでindex.htmlを作成

## 手順2
fork元のリポジトリを追加
```
git remote add upstream https://github.com/Tatsu0111/Kadai_fork.git
```
upstreamからfetchとmergeをしてローカルリポジトリを最新化
```
git fetch upstream
git merge upstream/main
```
作業ブランチを作成
```
git switch -c "sagyou1"
```
index.htmlを編集
```
echo "Add line 1" >> index.html
```
変更をコミットしてpush
```
git add index.html
git commit -m "手順２を実行"
git push origin sagyou1
```
upstreamのmainブランチを選びプルリクエストを作成
<img width="698" height="466" alt="スクリーンショット 2026-08-21 145506" src="https://github.com/user-attachments/assets/69184d36-5f01-4039-be8b-3dadcaefe960" />
___
<img width="882" height="751" alt="スクリーンショット 2026-08-21 145608" src="https://github.com/user-attachments/assets/c032aca5-4beb-4869-964c-a93909b72c8e" />


## 手順5
ローカルのmainブランチを最新化
```
git fetch upstream
git merge upstream/main
```
作業ブランチを作成
```
git switch -c sagyou3
```
stylesheet.cssを追加
```
echo "Hello" >> stylesheet.css
```
変更をコミットしてpush
```
git add stylesheet.css
git commit -m "手順５を実行"
git push origin sagyou3
```
upstreamのmainブランチを選びプルリクエストを作成
<img width="691" height="502" alt="スクリーンショット 2026-08-21 152714" src="https://github.com/user-attachments/assets/983a5230-bf54-4d98-9fd3-bce16eaff758" />
___
<img width="931" height="749" alt="スクリーンショット 2026-08-21 152733" src="https://github.com/user-attachments/assets/9648a82b-9c51-4e3c-bee3-fa631710752b" />


