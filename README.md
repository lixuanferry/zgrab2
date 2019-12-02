# zgrab2抓取标语、对标语分词、与指纹库匹配环境配置（Ubuntu 18.04.3 LTS）
## 1. 安装git
`sudo apt install git`
## 2. 安装go
`sudo add-apt-repository ppa:longsleep/golang-backports`
`sudo apt-get update`
`sudo apt-get install golang-go`
## 3. 安装zgrab2
`go get github.com/zmap/zgrab2`
###### 在src文件夹下新建golang.org/x
###### 进入x文件夹下
`git clone https://github.com/golang/sys.git`
`git clone https://github.com/golang/crypto.git`
`git clone https://github.com/golang/net.git`
`git clone https://github.com/golang/text.git`
`go get gopkg.in/mgo.v2/bson`
`go get gopkg.in/yaml.v2`
###### 进入zgrab2文件夹下
`make`
## 4. 安装open-vm-tools
`sudo apt install open-vm-tools`
`sudo apt install open-vm-tools-desktop    //双向拖放文件（可选）`
`sudo apt install open-vm-tools-dkms    //文件夹共享（可选）`
## 5. 安装pip
`sudo apt install python3-pip`
## 6. 安装ujson
`pip3 install ujson`
## 7. 安装nltk
`pip3 install nltk`
## 8. 安装nltk数据包
`import nltk`
`nltk.download('punkt')`
`nltk.download('stopwords')`
## 9. 抓取标语
`./zgrab2 multiple -c multiple.ini -o output.json -f /ip.json`
