# 手順

## 手順1
GitHub上にリモートリポジトリを用意
<img width="1672" height="458" alt="スクリーンショット 2026-08-21 145427" src="https://github.com/user-attachments/assets/c5443749-f7bb-4cf0-a8d2-e33244f10d59" />

<img width="730" height="926" alt="スクリーンショット 2026-08-21 140923" src="https://github.com/user-attachments/assets/215567b7-cd4e-4310-872b-a54662c1cd5d" />

cloneしローカルでindex.htmlを作成
```
git clone https://github.com/Tatsu0111/Kadai_fork
cd Kadai_fork/
echo "Hello" >> index.html
```

commitしmainブランチへpush
```
git add .
git commit -m "手順1を実行"
git push -u origin main
```

## 手順3
開発者側からのプルリクエストをレビュー
<img width="1510" height="427" alt="スクリーンショット 2026-08-21 145705" src="https://github.com/user-attachments/assets/e9cb9c87-efb0-4dab-9d48-e49dd764e88f" />

確認後mainブランチにマージ
<img width="1156" height="696" alt="スクリーンショット 2026-08-21 145714" src="https://github.com/user-attachments/assets/9cf58975-5789-43e3-892a-1b63c70df955" />
<img width="898" height="422" alt="スクリーンショット 2026-08-21 145724" src="https://github.com/user-attachments/assets/a350b3bc-deb3-47e1-8312-ce1af98a508b" />

## 手順4
ローカルのmainブランチを最新化し、作業ブランチを作成
```
git pull
git switch -c sagyo2
```

index.htmlを編集してリモートへpush
```
echo "Add line 2" >> index.html
git add index.html
git commit -m "手順4を実行"
git push origin sagyo2
```

プルリクエストを作成・マージ
<img width="1215" height="221" alt="スクリーンショット 2026-08-21 150048" src="https://github.com/user-attachments/assets/60edd888-bf58-4d60-ae60-72a0d98ae69c" />
<img width="936" height="669" alt="スクリーンショット 2026-08-21 150057" src="https://github.com/user-attachments/assets/b5e5e30d-dfca-427b-8f79-09b6bab3fe89" />
<img width="895" height="580" alt="スクリーンショット 2026-08-21 150110" src="https://github.com/user-attachments/assets/f2d8e002-921d-46e6-b373-3e5987b29b00" />
<img width="909" height="429" alt="スクリーンショット 2026-08-21 150116" src="https://github.com/user-attachments/assets/032b84ce-ce36-41fb-b1ce-16ecae2e44ba" />


## 手順6
開発者側からのプルリクエストをレビュー
<img width="1511" height="417" alt="スクリーンショット 2026-08-21 153326" src="https://github.com/user-attachments/assets/353e5a51-78e9-4ccc-a5a5-b888fb532e7a" />
確認後mainブランチにマージ
<img width="914" height="582" alt="スクリーンショット 2026-08-21 153335" src="https://github.com/user-attachments/assets/18cea39a-9e34-4ae9-8be2-86d3cba9d5c3" />
<img width="916" height="428" alt="スクリーンショット 2026-08-21 153340" src="https://github.com/user-attachments/assets/4ed59dd8-1ba9-46ba-b2f3-61e3557de8e3" />

