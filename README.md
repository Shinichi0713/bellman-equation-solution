## 目的

MDPの条件のもと導出したベルマン方程式を解くことで行動最適化が行われることを確認する。

ベルマン方程式の基本形
ベルマン方程式は次のように表されます：
V(s)=amax​[R(s,a)+γs′∑​P(s′∣s,a)V(s′)]

```math
(V(s)): 状態 (s) における価値関数（value function）。これは、状態 (s) から始めたときに得られる累積報酬の期待値を表します。
(a): 行動（action）。エージェントが取ることができる選択肢です。
(R(s, a)): 即時報酬（immediate reward）。状態 (s) で行動 (a) を取ったときに得られる報酬です。
(\gamma): 割引率（discount factor）。未来の報酬の現在価値を計算するための係数で、通常は (0 \leq \gamma < 1) の範囲で設定されます。
(P(s’|s, a)): 遷移確率（transition probability）。状態 (s) で行動 (a) を取ったときに次の状態 (s’) へ遷移する確率です。
(\sum_{s’}): 次の状態 (s’) についての総和を取ることを示します。
```

## 実験条件
以下の絵のS(状態)とa(行動)を選択の上、行動に対する最適な行動価値関数が得られることを確認する
![image](https://github.com/user-attachments/assets/dd39b572-3d8e-4bd7-a331-8b114297df63)



## 実行結果
step2で行動価値関数が収束した。
ベルマン方程式の解は最適化。
![image](https://github.com/user-attachments/assets/24b14174-9b32-4e87-b20b-e1c0ebe68058)

