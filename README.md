# learning-docker: Dockerの練習

## ミニレポート

### Q1-1: 同じ `docker container run` コマンドを2回実行すると、1回目と2回目で違いはありますか？どう違いますか？

【回答欄】
１回目：コンテナを作成するためのイメージをダウンロード　→echoコマンドを実行
２回目：即座にechoコマンドを実行

### Q1-2: なぜ違いますか？

【回答欄】
１回目はコンテナを作成するためのイメージをダウンロードする必要があるため

### Q1-3: `docker container ls` と `docker container ls -a` はどう違いますか？

【回答欄】
lsは現在起動しているコンテナを表示
ls -aは今までに作った全てのコンテナを表示


### Q1-4: `docker image ls` と `docker container ls -a` はどう違いますか？（間違ってもいいので、自分の考えを述べてください）

【回答欄】
前者はDocker Hubからダウンロードしてきたイメージ一覧を表示
後者はイメージをもとに作成したコンテナ一覧を表示

### Q1-5: `ubuntu` イメージでの `cat /etc/issue` の結果をペーストしてください

【回答欄】
Ubuntu 18.04.3 LTS \n \l

### Q1-6: `docker image ls` と `docker container ls -a` はどう変化しましたか？

【回答欄】
コンテナが１つ増えていた

### Q2-1: `-d` (デタッチド・モード) でコンテナを起動すると、どのような状態になりましたか？

【回答欄】
コンテナは作成されただけの状態？
ずっと起動している

### Q2-2: http://localhost/ をブラウザで開くと、何が表示されましたか？

【回答欄】
It works!
##うまく行ってないかも、、
Welcome to nginx!
#先生がやったらうまくいきました。ありがとうございます！！

###Q2-3: コンテナの起動時と終了時で、docker container ls -a はどのように変化しましたか？
ステータスがUpからExitedに変わった

### Q3-1: `docker build -t sample-image .` 実行時に表示されている `building...` は、Dockerfileのどの行から実行されましたか？

【回答欄】
12行目のRUN echo "building..."

### Q3-2: `docker run sample-image` を実行すると、どうなりましたか
【回答欄】
sample.rbが実行された