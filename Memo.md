# やったこと
まずはインストール方法: Gitからpullする．

```
$ git clone https://github.com/jMetal/jMetal
$ cd jMetal
```

EclipseかIntelliJかコマンドラインか迷う．Eclipseやってみよう．

## まずはEclipseで
実行できずに断念

## IntelliJで
DocumentにもあったのでIntelliJでやってみる

jMetalSample/jmetal-exec/src/main/java/org/uma/jmetal/runner/multiobjective/NSGAIIRunner.javaのmainを実行．

...エラー

xmlファイルがひらけない．

ツリーにディレクトリが表示されない．．．

`File`→`Project Structure`→`Modules`→`+`→`Import Module`→ファイル選択→`Import module from external model(Maven)`→`Next`...

実行(NSGAIIRunner)...

```
/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/bin/java "-javaagent:/Applications/IntelliJ IDEA.app/Contents/lib/idea_rt.jar=64775:/Applications/IntelliJ IDEA.app/Contents/bin" -Dfile.encoding=UTF-8 -classpath /Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/charsets.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/deploy.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/cldrdata.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/dnsns.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/jaccess.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/jfxrt.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/localedata.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/nashorn.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/sunec.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/sunjce_provider.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/sunpkcs11.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/ext/zipfs.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/javaws.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/jce.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/jfr.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/jfxswt.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/jsse.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/management-agent.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/plugin.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/resources.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/rt.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/ant-javafx.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/dt.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/javafx-mx.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/jconsole.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/packager.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/sa-jdi.jar:/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/lib/tools.jar:/Users/pyente/Github/jMetalSample/jmetal-core/target/test-classes:/Users/pyente/Github/jMetalSample/jmetal-core/target/classes:/Users/pyente/.m2/repository/junit/junit/4.11/junit-4.11.jar:/Users/pyente/.m2/repository/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.jar:/Users/pyente/.m2/repository/org/apache/maven/reporting/maven-reporting-api/3.0/maven-reporting-api-3.0.jar:/Users/pyente/.m2/repository/org/apache/maven/doxia/doxia-sink-api/1.0/doxia-sink-api-1.0.jar:/Users/pyente/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/Users/pyente/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/Users/pyente/.m2/repository/org/mockito/mockito-all/1.10.19/mockito-all-1.10.19.jar:/Users/pyente/.m2/repository/org/springframework/spring-test/4.0.7.RELEASE/spring-test-4.0.7.RELEASE.jar:/Users/pyente/.m2/repository/org/springframework/spring-core/4.0.7.RELEASE/spring-core-4.0.7.RELEASE.jar:/Users/pyente/.m2/repository/commons-logging/commons-logging/1.1.3/commons-logging-1.1.3.jar:/Users/pyente/.m2/repository/org/hamcrest/hamcrest-all/1.3/hamcrest-all-1.3.jar:/Users/pyente/.m2/repository/org/knowm/xchart/xchart/3.2.2/xchart-3.2.2.jar:/Users/pyente/.m2/repository/de/erichseifert/vectorgraphics2d/VectorGraphics2D/0.11/VectorGraphics2D-0.11.jar:/Users/pyente/.m2/repository/org/apache/commons/commons-math3/3.6.1/commons-math3-3.6.1.jar:/Users/pyente/.m2/repository/nz/ac/waikato/cms/weka/weka-stable/3.8.1/weka-stable-3.8.1.jar:/Users/pyente/.m2/repository/nz/ac/waikato/cms/weka/thirdparty/java-cup-11b/2015.03.26/java-cup-11b-2015.03.26.jar:/Users/pyente/.m2/repository/nz/ac/waikato/cms/weka/thirdparty/java-cup-11b-runtime/2015.03.26/java-cup-11b-runtime-2015.03.26.jar:/Users/pyente/.m2/repository/nz/ac/waikato/cms/weka/thirdparty/bounce/0.18/bounce-0.18.jar:/Users/pyente/.m2/repository/com/googlecode/matrix-toolkits-java/mtj/1.0.4/mtj-1.0.4.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-osx-x86_64/1.1/netlib-native_ref-osx-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/native_ref-java/1.1/native_ref-java-1.1.jar:/Users/pyente/.m2/repository/com/github/fommil/jniloader/1.1/jniloader-1.1.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-linux-x86_64/1.1/netlib-native_ref-linux-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-linux-i686/1.1/netlib-native_ref-linux-i686-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-win-x86_64/1.1/netlib-native_ref-win-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-win-i686/1.1/netlib-native_ref-win-i686-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_ref-linux-armhf/1.1/netlib-native_ref-linux-armhf-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-osx-x86_64/1.1/netlib-native_system-osx-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/native_system-java/1.1/native_system-java-1.1.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-linux-x86_64/1.1/netlib-native_system-linux-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-linux-i686/1.1/netlib-native_system-linux-i686-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-linux-armhf/1.1/netlib-native_system-linux-armhf-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-win-x86_64/1.1/netlib-native_system-win-x86_64-1.1-natives.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/netlib-native_system-win-i686/1.1/netlib-native_system-win-i686-1.1-natives.jar:/Users/pyente/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/Users/pyente/.m2/repository/com/googlecode/netlib-java/netlib-java/1.1/netlib-java-1.1.jar:/Users/pyente/.m2/repository/com/github/fommil/netlib/core/1.1/core-1.1.jar:/Users/pyente/Github/jMetalSample/jmetal-problem/target/test-classes:/Users/pyente/Github/jMetalSample/jmetal-problem/target/classes:/Users/pyente/Github/jMetalSample/jmetal-algorithm/target/test-classes:/Users/pyente/Github/jMetalSample/jmetal-algorithm/target/classes:/Users/pyente/.m2/repository/org/mockito/mockito-core/1.10.8/mockito-core-1.10.8.jar:/Users/pyente/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/Users/pyente/Github/jMetalSample/jmetal-exec/target/classes org.uma.jmetal.runner.multiobjective.NSGAIIRunner
objc[13595]: Class JavaLaunchHelper is implemented in both /Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/bin/java (0x10c9574c0) and /Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home/jre/lib/libinstrument.dylib (0x10c9db4e0). One of the two will be used. Which one is undefined.
2018-09-12 03:06:39.513 INFO: Loggers configured with null [org.uma.jmetal.util.JMetalLogger configureLoggers]
2018-09-12 03:06:39.581 INFO: Total execution time: 2694ms [org.uma.jmetal.runner.multiobjective.NSGAIIRunner main]
2018-09-12 03:06:39.625 INFO: Random seed: 1536689196805 [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 03:06:39.626 INFO: Objectives values have been written to file FUN.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 03:06:39.627 INFO: Variables values have been written to file VAR.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 03:06:39.940 INFO:
Hypervolume (N) : 0.6595303893415901
Hypervolume     : 0.6595303893415901
Epsilon (N)     : 0.011676587061837697
Epsilon         : 0.011676587061837697
GD (N)          : 2.540921634743263E-4
GD              : 2.540921634743263E-4
IGD (N)         : 1.8643051624714905E-4
IGD             : 1.8643051624714905E-4
IGD+ (N)        : 0.0037425108310230708
IGD+            : 0.0037425108310230708
Spread (N)      : 0.4118010288844388
Spread          : 0.4118010288844388
Error ratio     : 1.0
 [org.uma.jmetal.util.AbstractAlgorithmRunner printQualityIndicators]

Process finished with exit code 0
```

無事にできてなによりです．

## 最終手段コマンドライン
`brew install maven`でmavenダウンロード．

- とりあえず，`mvn clean`
- コンパイル: `mvn compile`
- テスト: `mvn test`
- なんやかんや: `mvn package`
- サイト？: `mvn site`

```
$ mvn package
$ java -cp jmetal-exec/target/jmetal-exec-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-core/target/jmetal-core-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-problem/target/jmetal-problem-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-algorithm/target/jmetal-algorithm-5.7-Beta-35-jar-with-dependencies.jar org.uma.jmetal.runner.multiobjective.NSGAIIRunner org.uma.jmetal.problem.multiobjective.zdt.ZDT1
Error: Could not find or load main class org.uma.jmetal.runner.multiobjective.NSGAIIRunner
```

ん？

```
$ java -cp jmetal-exec/target/jmetal-exec-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-core/target/jmetal-core-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-problem/target/jmetal-problem-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-algorithm/target/jmetal-algorithm-5.7-Beta-35-jar-with-dependencies.jar org.uma.jmetal.runner.multiobjective.NSGAIIRunner org.uma.jmetal.problem.multiobjective.zdt.ZDT1
2018-09-12 02:39:52.835 INFO: Loggers configured with null [org.uma.jmetal.util.JMetalLogger configureLoggers]
2018-09-12 02:39:52.951 INFO: Total execution time: 697ms [org.uma.jmetal.runner.multiobjective.NSGAIIRunner main]
2018-09-12 02:39:53.058 INFO: Random seed: 1536687592126 [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 02:39:53.059 INFO: Objectives values have been written to file FUN.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 02:39:53.061 INFO: Variables values have been written to file VAR.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
```

```
java -cp jmetal-exec/target/jmetal-exec-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-core/target/jmetal-core-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-problem/target/jmetal-problem-5.7-SNAPSHOT-jar-with-dependencies.jar:jmetal-algorithm/target/jmetal-algorithm-5.7-Beta-35-jar-with-dependencies.jar org.uma.jmetal.runner.multiobjective.NSGAIIRunner org.uma.jmetal.problem.multiobjective.zdt.ZDT1 jmetal-problem/src/test/resources/pareto_fronts/ZDT1.pf
2018-09-12 02:43:01.945 INFO: Loggers configured with null [org.uma.jmetal.util.JMetalLogger configureLoggers]
2018-09-12 02:43:02.003 INFO: Total execution time: 729ms [org.uma.jmetal.runner.multiobjective.NSGAIIRunner main]
2018-09-12 02:43:02.060 INFO: Random seed: 1536687781206 [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 02:43:02.063 INFO: Objectives values have been written to file FUN.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 02:43:02.066 INFO: Variables values have been written to file VAR.tsv [org.uma.jmetal.util.AbstractAlgorithmRunner printFinalSolutionSet]
2018-09-12 02:43:02.355 INFO:
Hypervolume (N) : 0.6588037170769601
Hypervolume     : 0.6588037170769601
Epsilon (N)     : 0.014822684880191617
Epsilon         : 0.014822684880191617
GD (N)          : 2.1875332381049724E-4
GD              : 2.1875332381049724E-4
IGD (N)         : 1.9732405659050572E-4
IGD             : 1.9732405659050572E-4
IGD+ (N)        : 0.004158193353486375
IGD+            : 0.004158193353486375
Spread (N)      : 0.42886979484964705
Spread          : 0.42886979484964705
Error ratio     : 1.0
 [org.uma.jmetal.util.AbstractAlgorithmRunner printQualityIndicators]
```

どう見ればいいのか…
