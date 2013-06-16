KnowledgeInterDisciplinary
=================

```
#!/bin/bash

#json_path=./KnowledgeInterDisciplinary

json_path=~/repos/KnowledgeInterDisciplinary



for i in `ls -Rt $json_path | egrep -i "\(" | sed s'/.json//'i  | sed s'/^.*.(//' | tr -d "()" | sort -u`; do  qq=$(ls $json_path/data/*json | grep $i); for f in $qq;do echo  '"path":'$json_path',"category:'$i'",name:"'$f'",'; done done


```
