### 2019-Viphakone:  Co-transcriptional Loading of RNA Export Factors
Shapes the Human Transcriptome

https://doi.org/10.1016/j.molcel.2019.04.034


### 2019-Lee: Pericentromeric heterochromatin is hierarchically organized and spatially contacts H3K9me2/3 islands located in euchromatic genome

http://dx.doi.org/10.1101/525873

ハエの pericentromeric heterochromatin に注目した Hi-C。***TODO***


### 2019-Susman: Stable memory with unstable synapses

https://doi.org/10.1038/s41467-019-12306-2

記憶ニューロンの数理モデル。外場 b(t) と隣接行列 W(t) を使って記述される力学系 dx/dt = -x + W(t)φ(x) + b(t) の動的なリミットサイクルとして現れる記憶現象を解析。W(t) の固有値の虚部 (つまりグラフエッジの非対称性) が記憶を司ることを見つけた。

感想: おもしろ。ネットワークの記憶と想起ってこんなふうに計算でシミュレート出来るのか。GRN にも応用できる話だし夢ある。この計算においてノイズはどんだけ重要なのかはよく分からなかった。


### 2019-Ramaswamy: Learning protein conformational space by enforcing physics with convolutions and latent interpolations

https://arxiv.org/abs/1910.04543

CNN ベースの VAE による蛋白質遷移状態の構造予測。蛋白質の2種類の安定状態の構造を学習させ、その間の未観測の遷移状態をラテント変数から生成する。デコーダロスが物理的で、原子の結合長、結合角、LJ 相互作用、クーロン相互作用を取り込んでいる。さらに入力した2つの構造 x1, x2 のラテント表現 z1, z2 の再構築ロスだけでなく、z1, z2 を結ぶ線上でロス関数を積分して使うので物理的に妥当な遷移状態が予測できるという触れ込み。

感想: おもしろ。この論文の段階だと、モデルが物理を学習するにはサンプルが少なすぎだし、ラテント空間の線分を使ってるせいか状態遷移のパスが単純すぎる気がする。でも物理を理解する VAE で未観測状態を内挿するっていう姿勢は好きだし、有用そうだと思った。


### 2019-Tan: EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks

https://arxiv.org/abs/1905.11946

CNN のハイパーパラメータ選択指針。Depth d (層数)、width w (フィルタ数)、resolution r (入力画像のサイズ; ピクセル数でなくスケール) はスケーリング則に従って決めると、より少ない計算量で良い結果が出せる。いわく、α β^2 γ^2 = 2 に従うパラメータ α, β, γ および φ を選び、d = α^φ, w = β^φ, r = γ^φ の形で CNN のハイパーパラメータを決めると良いらしい。理論は無い。

感想: 理論が欲しい。CNN 以外のアーキに応用するには? 画像でなく時系列シグナルの場合は?

### 2012-Hinde: Tracking the mechanical dynamics of human embryonic stem cell chromatin

https://doi.org/10.1186/1756-8935-5-20

クロマチン動態の蛍光トラッキング。hESC と HeLa の DNA を Hoechst 染色して、高速ラインスキャンにより線分上のクロマチン分布を時系列で計測する。一次元だがクロマチンの動態を解析できる。時間相関 G(τ) を計算すると、未分化の hESC では ATP に依存した 10-100 Hz の振動 (breathing) が存在することが分かった。

感想: へぇ。


### 2017-Nozaki: Dynamic Organization of Chromatin Domains Revealed by Super-Resolution Live-Cell Imaging

https://doi.org/10.1016/j.molcel.2017.06.018

ヌクレオソーム動態の蛍光観察。ヌクレオソーム集団の RDF、MSD，L-function を解析している。***TODO***

感想: 分裂期と間期でヌクレオソームのドメインサイズが同じということは、ドメイン程度のサイズで粗視化したクロマチンビーズの半径は不変でよいのか?


### 2018-Huaa: Mitotic antipairing of homologous and sex chromosomes via spatial restriction of two haploid sets

https://doi.org/10.1073/pnas.1809583115

染色体ペインティング。マウスとヒトの分裂期 (meta-anaphase) において相同染色体が核の反対側 (hemisphere) に配置されることを見つけた。性染色体でもそうなる。望まれない交叉を防ぐために相同染色体を空間的に分離しておく機構があるのだろうと言っている。間期の様子は実験手法の限界ではっきりとは分からなかったそうだが、おそらく半球分離みたいな激しいことにはなっていないだろうとのこと。

感想: ヒトゲノムの三次元構造をモデリングするとき、相同染色体は鏡面対称に配置すべきかも?
