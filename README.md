
## Unity＋OculusによるVR開発について

Unity＋Oculusの開発記事に技術検証を付け加えたメモ書きになります。<br>
最初にVR開発において以下の二つの手法があります。

* ①Oculus＋PC(PCVR)で動作させる場合<br>
* ②Oculus単機で動作させる場合<br>


どちらにもメリット・デメリットがあります

---

#### ①Oculus＋PC(PCVR)で動作させる場合

PCVRで動作させる場合すべての処理が接続されているPC(動作させるPC)に依存します。<br>
参考までにPCVRに必要最低限のスペックが以下の通りです


| CPU | Intel i5-490 |
|:---:|:---:|
| GPU | GTX 1060 |
| RAM | 8GB |
| USBケーブル | 必要に応じて |
| Wifi | 5Ghz |


※引用(https://drone-guide.org/oq2-pcvr-spec/)


#### ②Oculus単機で動作させる場合

Oculus単体で立ち上げる場合動作の処理はすべてOculus側で行います。<br>
そのため動作が個々の機器によって異なるという
