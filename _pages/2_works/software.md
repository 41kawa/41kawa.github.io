---
layout: page
title: 研究成果
permalink: /works/software/
---

## ソフトウェア/ツール

### JAXとJIT compilerで高速化したテンソル因子分解ライブラリ [[GitHub](https://github.com/tokyotech-nakatalab/tensor-decomposition){:target="_blank"}]

#### 水谷圭佑 (2023).

テンソル因子分解，非負克テンソル因子分解，ポアソンテンソル因子分解，ゼロ過剰ポアソンテンソル因子分解を実装しています．

### SCOPE-RL [[GitHub](https://github.com/hakuhodo-technologies/scope-rl){:target="_blank"}, [PyPI](https://pypi.org/project/scope-rl/){:target="_blank"}, [Documentation](https://scope-rl.readthedocs.io/en/latest/){:target="_blank"}]

#### Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, and Yuta Saito (2023).

SCOPE-RLは，オフライン強化学習や，そのオフラインでの性能評価・モデル選択の実装を一貫して行えるライブラリです．特にオフライン評価に関する実装に力を入れており，方策の期待性能を評価する従来の手法のほかに，性能分布全体を評価する最先端の研究や，さらには数々のオフライン評価指標を多角的に性能検証するための機能までをも実装しています．

- [博報堂テクノロジーズからのプレスリリース](https://prtimes.jp/main/html/rd/p/000000007.000113498.html){:target="_blank"}

### IPCPrediction [[GitHub](https://github.com/tokyotech-nakatalab/IPCPrediction){:target="_blank"}]

#### 星野雄毅, 中田和秀 (2021).

[IPC prediction of patent documents using neural network with attention for hierarchical structure](https://doi.org/10.1371/journal.pone.0282361){:target="_blank"}での実験を再現することができます．

### BCDSNL [[GitHub](https://github.com/xidaogy/BCDSNL){:target="_blank"}]

#### 西島光洋, 中田和秀 (2021).

[A block coordinate descent method for sensor network localization](https://doi.org/10.1007/s11590-021-01762-9){:target="_blank"}での実験を再現することができます．

### MDRRT-scheduling-dwave [[GitHub](https://github.com/MK-tech20/MDRRT-scheduling-dwave){:target="_blank"}]

#### 倉又迪哉, 香月諒太, 中田和秀 (2021).

[Solving large break minimization problems in a mirrored double round-robin tournament using quantum annealing](https://doi.org/10.1371/journal.pone.0266846){:target="_blank"}での実験を再現することができます．

### PCMF [[GitHub](https://github.com/N-YS-KK/PCMF){:target="_blank"}, [PyPI](https://pypi.org/project/pcmf/){:target="_blank"}]

#### 住谷有規, 松井諒生, 近藤謙将, 中田和秀 (2021).

PCMF（Positive Collective Matrix Factorization）は，推薦システムや画像・テキストの解析など多岐にわたり適用される「行列因子分解（Matrix Factorization）」に基づいた手法です．既存の手法であるNMF（Non-Negative Matrix Factorization）の解釈可能性とCMF（Collective Matrix Factorization）の拡張性を兼ね備えたモデルとなっています．

- ☆[Patient disease prediction and medical feature extraction using matrix factorization](https://www.jstage.jst.go.jp/article/pjsai/JSAI2021/0/JSAI2021_2G3GS2e03/_pdf/-char/ja){:target="_blank"}

### CGA2M+ [[GitHub](https://github.com/MK-tech20/CGA2M_plus){:target="_blank"}, [PyPI](https://pypi.org/project/cga2m-plus/){:target="_blank"}]

#### 倉又迪哉, 渡邊彰久, 馬嶋海斗, 清原明加, 近藤謙将, 中田和秀 (2021).

Constraint GA2M plus（CGA2M+）は，予測に対する解釈性と予測精度を両立したモデルです．単調性の導入と高次の相互作用の考慮の2点の改良を既存の手法であるGA2Mに施し，解釈性と予測精度を高めました．

- [Constrained generalized additive 2 model with consideration of high-order interactions](https://doi.org/10.1109/ICECET52533.2021.9698779){:target="_blank"}

### Cardinality-constrained CVaR Optimization [[GitHub](https://github.com/KenKoba2119/cardinality-constrained_cvar_optimization){:target="_blank"}]

#### 小林健 (2020).

[Bilevel cutting-plane algorithm for solving cardinality-constrained mean-CVaR portfolio optimization problems](https://doi.org/10.1007/s10898-021-01048-5){:target="_blank"}での実験を再現することができます．

### Structure-emphasized Multimodal Style Transfer [[GitHub](https://github.com/irasin/Structure-emphasized-Multimodal-Style-Transfer){:target="_blank"}]

#### 陳晨 (2020).

コンテンツ画像と画風を表すスタイル画像を与えて，スタイル画像の持つ画風をコンテンツ画像に移した新しい画像を生成するために，事前に学習されたモデルを提供しています．

### QuantOnline

#### 藤森和哉, 中田和秀 (2012).

QuantOnlineは，金融工学分野での計算をオンラインで行うインフラです．その内部は，金融数値計算のベースに実務でも数多くの企業に採用されているライブラリQuantLibを使用し，数式処理のベースに汎用数式処理システムMaximaを使用しています．

- セキュリティ上の理由で，現在は運用を休止中．
