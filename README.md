# jupyter-vagrant

任意の場所に新規にディレクトリを作成します。
そのディレクトリにVagrantfile, pull_image.sh, run.shのファイルをコピーします。
そのディレクトリで次のコマンドを実行すると、Jupyter用の仮想マシンが作成され起動します。

`vagrant up`

初回の起動時は、仮想マシンのOSとJupyter関連のデータのダウンロードに時間がかかります。（おおよそ5GBはあります）

完了後にブラウザで `http://localhost:8888/` にアクセスするとJupyter notebookを使用できます。
