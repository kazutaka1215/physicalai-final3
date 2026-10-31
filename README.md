# PAI最終課題 

YOLOv8nで物体を検出し、色ルールで赤/青の箱へ仕分けるタスク。
2次元簡易シミュレーション上で、75秒間に20個を仕分け。

## 実行
`task04_sort4.ipynb` を Google Colab で開き、上から順に実行。

## 使用技術
Python, numpy, matplotlib（Colab無料枠）、2リンクIK

## AI活用
YOLOv8n（推論のみ）で検出 → 色ルールで仕分け先を決定。

## 工夫点
- 速度制限補間でアームをゆっくり動かし目視しやすく
- 状態機械（idle→pick→carry→place）で安定管理
- 箱を到達圏内に配置し、収まりを可視化
