### 2017-Dillinger: Nucleolus association of chromosomal domains is largely maintained in cellular senescence despite massive nuclear reorganisation

https://doi.org/10.1371/journal.pone.0178821


### 2019-Graf: Xor Filters: Faster and Smaller Than Bloom and Cuckoo Filters

https://arxiv.org/abs/1912.08258

ブルームフィルタ的なデータ構造。既知要素のフィンガープリントを複雑なアルゴリズムで3つのハッシュ配列に登録する。クエリ時は3つのハッシュ配列からクエリキーの値を取り出して xor をとり、結果がクエリキーのフィンガープリントに一致するかどうかをテストする。同一ビット数ならブルームフィルタより偽陽確率が低く優秀。

感想: RAID でパリティを分散させるような考え方で面白い。クエリだけなら好き。でもフィルタ構築アルゴリズムが複雑で嫌だ。[HN](https://news.ycombinator.com/item?id=21840821) あり。


### 2019-Ngai: Absolutely necessary to consider the caged dynamics and the JGX β-relaxation in solving the glass transition problem 

https://doi.org/10.5488/CMP.22.43605

ガラス転移のオピニオン論文。α/βJGX-緩和過程において caged dynamics (MSD ⟨u^2⟩ の挙動) が重要であるという主張。⟨u^2(Tg)⟩ (散乱実験で測定される ~1ns 以下の MSD) が α-転移の指数パラメータ n と相関する、Tg 前後で ⟨u^2(T)⟩ の温度依存性が変わる、β-緩和時間で ⟨u^2(t)⟩ の指数が変化する (caging が終わる) など。遅いガラス転移を理解するためには caged dynamics のような速い過程の理解が重要だと主張する。

感想: タイトル必死w でも面白い。つっかえて動けなかったり急に動いたりするのはイメージ的にガラスぽいわけで、関係あるだろうとは思う。何が起こってるのか気になる。


### 2019-Potapova: Superresolution microscopy reveals linkages between ribosomal DNA on heterologous chromosomes

https://doi.org/10.1083/jcb.201810166

ヒト rDNA に注目した細胞核の超解像実験。間期と分裂期において異なる染色体の rDNA どうしが「リンク」する様子を調べている。リンク形成には UBF が必須で、rDNA の転写が多いほど (iPS, c-Myc++) リンクは生じやすく、topo II が無いと細胞分裂時にリンクが解けない。リンクの正体は明確ではないが繊維状の何かで、著者は rDNA だと推測している。著者のモデルは、混雑した核小体内で rDNA が topo II の効果により絡まり、分裂時に解消されるというものだ。

感想: ほほう系面白い。ヒトの核で核小体が少数にまとまるのは、マクロな相分離でなく親細胞の核小体の記憶が rDNA のリンクによって残ってるからなのかも。あとこの論文は核小体の画像がたくさん載っていてイメージふくらむのが良い。


### 2018-Petersen: Topological properties of the set of functions generated by neural networks of fixed size

https://arxiv.org/abs/1806.08459

NN で実現される関数空間の数理。レイヤ数 L とニューロン数 N を固定したとき、活性化関数 σ を使ったアーキテクチャ S で実現される関数の集合を RNNσ(L,N) と書く。このとき、RNNσ(L,N) は Lp 空間の閉じた集合ではないことが示される。つまり学習したい関数が RNNσ(L,N) 内の点列の極限として実現できない (学習不可能) ことがある。ただし σ=ReLU の場合のみ L∞ 空間で閉じている可能性があるそうだ (一般の証明はできなかったが、2層 NN では証明できた)。また、重みから Lp 関数への写像は連続だが、逆写像は連続でないことも示される。

感想: 面白い結果だが証明は追えん。


### 2018-Huang: Densely Connected Convolutional Networks

https://arxiv.org/abs/1608.06993

ResNet の改良版 CNN アーキテクチャ。スキップ接続を add でなく concat オペレーションにする。Dense Block という数十レイヤーの単位で concat を重ねて幅を広げ、Translation Layer でいったん接続を切り次元を下げる、というのを繰り返す構造。WRN と違って各レイヤーの width (フィルタ数; growth rate k) を小さく出来る。ImageNet において ResNet 並の成績を半分のパラメータ数や FLOP 数で実現した。

感想: 技術的には順当な一般化だ。ブロックに分けて次元が上がりすぎないようにするのも順当だけど、言うは易し。うまくいくやり方を見つけてくれたのは大きい。著者も議論してるが、DenseNet は ResNet とは本質的に違って、差分を学習するのでなく徹底的に feature reuse をするのがポイントなのかもしれない。各レイヤが小さな学習をして、その寄せ集めで良い成績を出すという。


### 2015-Young: Regulation of the Epigenome by Vitamin C

https://dx.doi.org/10.1146/annurev-nutr-071714-034228

ビタミンCのエピジェネティクス視点でのレビュー。ビタミンCは (1) DNA脱メチル化酵素 TIT の補酵素および (2) ヒストン (H3K9/36) 脱メチル化酵素の補酵素として使われる (鉄イオンのからんだ redox に使われるらしい)。癌細胞、神経細胞、iPS 細胞の話題も出ている。

感想: 鬼おもしろい。ビタミンCは免疫に必要というより、一般にエピジェネティック調節 (特にリプログラミング) に必要な因子なのかもしれない。免疫でのビタミンCの役割も結局、T細胞のエピゲノムを完成させ維持するのに必要だということか。知識が一般化されて賢くなったような気分だ。


### 2013-Manning: Vitamin C Promotes Maturation of T-Cells

https://dx.doi.org/10.1089/ars.2012.4988

ビタミンCがT細胞分化に必要であるという実験。リンパ芽球のT細胞 (キラーとか) への分化は CD4, CD8 という2つの抗体遺伝子の発現 (DP; double positiblve) により特徴づけられる。論文の実験では未分化の細胞をビタミンCありの条件 (pAsc) とコントロールで培養。フローサイトメトリーで抗体の発現量を測定した結果、pAsc 条件のときのみ DP が現れ、しかもpAsc 供給を継続しないと DP は維持できないと分かった。マイクロアレイによると発現量が変化したのは CD8 だった。また ChIP-seq の結果、pAsc 条件では CD8 遺伝子プロモータ領域の H3K9me2 が減少することが分かった。

感想: 面白い。ビタミンCが免疫力を高めるという話に関わるきちんとした、筋の通せそうな話だ。 CD8 のエピジェネティック調節に効き、それによりT細胞の分化成熟と活性維持に効いているのか。


### 2019-Barrington: Enhancer accessibility and CTCF occupancy underlie asymmetric TAD architecture and cell type specific genome topology

https://doi.org/10.1038/s41467-019-10725-9


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
