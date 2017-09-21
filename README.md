# docker-jupyter
機械学習関連のライブラリとjupyter notebookをさっと使えるようにしたdocker imageです。

## 使い方
こんな感じで使ってください。

```
docker run --name "jupyter" --rm -it -p 8889:8888 -v ~/Dropbox/jupyter_notebooks/:/tmp yasuhisa/jupyter jupyter notebook --allow-root --ip=0.0.0.0 --NotebookApp.token='' --notebook-dir='/tmp/'
```
