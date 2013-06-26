KnowledgeInterDisciplin
=================

```
#!/bin/bash

#json_path=./KnowledgeInterDisciplinary

json_path=~/repos/KnowledgeInterDisciplinary/data/json



for i in `ls -Rt $json_path | egrep -i "\(" | sed s'/.json//'i  | sed s'/^.*.(//' | tr -d "()" | data-freq`; do  for f in $qq;do echo  '"path":'$json_path',"category:'$i'",name:"'$f'",'; done done


```
