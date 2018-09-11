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
