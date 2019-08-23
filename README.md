# jekins-checkout-plugin
Jenkins 检查 pom.xml 插件
如果勾选了复选框，它将检查 pom.xml 中是否包含 SNAPSHOT。


如果匹配，该次构建将被标记为失败。

流水线 job 使用
step([$class: 'MavenSnapshotCheck', check: 'true'])

如何构建及测试？
构建插件：
mvn package

本地测试（调用本地附带了该插件的 Jenkins 实例）；
mvn hpi:run
