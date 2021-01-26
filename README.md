# version
python: 3.9

# package

# setup

## mecab-ipadicのインストール
```bash
brew install mecab
brew install mecab-ipadic
git clone https://github.com/neologd/mecab-ipadic-neologd.git
mecab-ipadic-neologd/bin/install-mecab-ipadic-neologd -n
rm -r mecab-ipadic-neologd
```
## wnjpn.dbのダウンロード
```bash
curl http://compling.hss.ntu.edu.sg/wnja/data/1.1/wnjpn.db.gz --output "Clustering/wnjpn.db.gz"
gzip -d Clustering/wnjpn.db.gz
```

# アプリケーションの実行
```bash
make main
```