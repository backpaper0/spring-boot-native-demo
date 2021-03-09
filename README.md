
次のウェブページを参考にしてSpring Bootアプリケーションをネイティブビルドしてみた。

- https://docs.spring.io/spring-native/docs/current/reference/htmlsingle/#getting-started-native-image


GraalVM CEを任意の場所へインストール。

- https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-21.0.0.2

`bin`ディレクトリに`gu`コマンドがあるので、それを使って`native-image`コマンドをインストール。

```
gu install native-image
```

`JAVA_HOME`にGraalVM CEの場所を設定して`mvn package`すると`target`ディレクトリへバイナリが出力される。

