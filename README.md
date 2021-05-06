# demo

## Spring bootでWebアプリケーションを最速立ち上げするデモプロジェクト

- ビルドツール:Maven
- Javaバージョン:12
- とりあえずローカルで実行してhttp://localhost:8080/にアクセスしたらhelloが出るよ。
- コントローラにリクエストを飛ばす方法は、@RequestMapping(value="/", RequestMethod.GET)
- valueの部分を変えれば、呼び出すためのHTTPリクエストのURLも変化するよ。
  - 例えば、value="/api"ならhttp://localhost:8080/api/で呼び出せるよ。
  - RequestMethod.PUTとかGET以外にも書き込み指示を送れたりするよ。
- コントローラでreturnした文字が呼び出すhtml名になるよ。
- コントローラでmodelにaddAtributeで必要な情報を詰めてあげると、thymeleafでは${キー名}で呼び出せるよ。
