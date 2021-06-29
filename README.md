# split-gpx
gpxを分割するスクリプトです。

●ここから先は通ったことが無いから「どの道通った」の入力に使いたい

$ perl split-gpx 20210605111759.gpx 35.549297° 139.534828°

分割したい場所を緯度経度で指定。GPX Viewerの緯度経度が表示されているところをタップしてコピペ。
指定した場所周辺の半径50mに入ったところで、ファイルを分割。

●ここから先は通ったことがあるから「どの道通った」の入力に使いたくない

$ perl split-gpx2 20210605111759g.gpx 35.659673° 139.532915°

指定した場所周辺の半径50mに入った後出たところで、ファイルを分割。

分割の際はファイル名の末尾にfとgを付けます。短いことでAndroidのTermuxでも扱いやすくしてます。

どの道通った
https://matchansk.sakura.ne.jp/gpsc/

These scripts split your gpx file at the point you specify with its latitude and longitude.
