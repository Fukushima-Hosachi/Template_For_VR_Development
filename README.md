
## OculusによるVR開発について

Unity＋Oculusの開発記事に技術検証を付け加えたメモ書きになります。<br>
最初にVR開発において以下の二つの手法があります。

* ①Oculus＋PC(PCVR)で動作させる場合<br>
* ②Oculus単機で動作させる場合<br>


どちらにもメリット・デメリットがあります

---

#### ①Oculus＋PC(PCVR)で動作させる場合

PCVRで動作させる場合すべての処理が接続されているPC(動作させるPC)に依存します。<br>
参考にPCVRに必要最低限のスペックが以下の通りです。

| パーツ | 型番 |
|:---:|:---:|
| GPU | GTX 1060 |
| RAM | 8GB |
| USBケーブル | 必要に応じて |
| Wifi | 5Ghz |

>引用(https://drone-guide.org/oq2-pcvr-spec/)

そんなに高いスペックは求められませんが高処理をかけた場合、こちらで動いたがあちらで動かないということもしばしばあります。<br>


代表例：SteamVR　<img src="https://user-images.githubusercontent.com/71868188/196950937-8f69f3a5-e0f8-4b58-870e-191b4965da50.png" width="360px"> 

` メリット： デバッグが簡単、高処理をかけられる`  
` デメリット： 機材によって動作が変わる `

----

#### ②Oculus単機で動作させる場合

Oculus単体で立ち上げる場合動作の処理はすべてOculus側で行います。<br>
そのため動作が個々の機器によって異なるということはありません。<br>
一方で

代表例：Cluster
<img src="https://user-images.githubusercontent.com/71868188/196956041-6af08fd1-9546-47bc-85c3-842d53d4f0e1.png" width="360px">
YoutubeVR
<img src="https://user-images.githubusercontent.com/71868188/196956492-6f98f2ed-32df-4ca0-801e-b40ae075ff91.png" width="360px">

` メリット： 個々の機材で違う動作が起こることは少ない `  
` デメリット：Oculus側へのデプロイ方法が曖昧。Oculus Link(有線接続)よるデプロイ方法であるためゲーブルが必須 `




## Unity＋OculusによるVR開発詳細について

続いてUnity＋OculusによるVR開発についてです。<br>
以上２つの方法の動作方法がありますが、上記内容を踏まえてPCVRによる開発を前提に環境構築・技術検証を行った。

>参考元(https://qiita.com/pira/items/1c935f30d5ba6c020333)

1. 環境構築  
 ・使用したもの  
   機材関係：OculusQuest2、Unity 2021.3.9f1、デスクトップPC  
   プラグイン関係：

2. 
