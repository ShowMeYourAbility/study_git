初始状态为：main分支只有一个hello.txt文件，文件内容为c1
study_push00用于指定当前初始状态的节点
study_push01在初始状态下,hello.txt文件中新增一行c01,并执行git push -u origin study_push01
study_push02在初始状态下,hello.txt文件中新增一行c02,并执行git push -u origin study_push02:study_push01。看下这种场景的 push 是什么效果？
study_push03在初始状态下新增一个文件hello03.txt，文件内容任意如c1，并执行git push -u origin study_push03
study_push04在初始状态下新增一个文件hello04.txt，文件内容任意如c1，并执行git push -u origin study_push04:study_push03。看下这种场景下的 push 是什么效果？
将main分支同时push到gitee上

最佳实践：
git push -u 只用于本地与远程同名分支的场景，其他稀奇古怪的对应关系不要考虑
将main分支同时push到gitee和github上是可行的

如果我先后执行了git push -u origin main 和 git push -u origin_gitee main后，后续git push 是以哪个为准呢？
经试验：后面关联的同名远程分支会覆盖之前的同名名远程关联
