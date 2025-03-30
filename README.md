# packer-config
Vagrant用のboxファイル作成時に使用する、Packerの設定ファイルを置いてます。
徐々にOSを増やしていく予定です。



## 環境
```
packer --version
Packer v1.12.0
```


## Ubunutuについて
Ubuntuについては、どうやら`22.04 LTS`以降より`live-server ISO`での提供のみになってしまったようです。  
ですので`22.04 LTS`以降ではPreseedではなくautoinstallで行っています。  
（噂によればPreseedでも行けるとか…ただautoinstallの方がわかりやすいです。）

後、メモリを1Gにすると`curtin in-target`で異様に時間がかかる、最悪は進まなくなってしまうので2Gとしています。