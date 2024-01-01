初始状态为：main分支只有一个hello.txt文件，文件内容为c1
study_push00用于指定当前初始状态的节点
study_push01在初始状态下,hello.txt文件中新增一行c01,并执行git push -u origin study_push01
study_push02在初始状态下,hello.txt文件中新增一行c02,并执行git push -u origin study_push02:study_push01。看下这种场景的 push 是什么效果？
study_push03在初始状态下新增一个文件hello03.txt，文件内容任意如c1，并执行git push -u origin study_push03
study_push04在初始状态下新增一个文件hello04.txt，文件内容任意如c1，并执行git push -u origin study_push04:study_push03。看下这种场景下的 push 是什么效果？
将main分支同时push到gitee上
