# manifests
如无必要,勿增实体

1. 0repoinit:

```
#!/bin/bash

git_host=git@github.com:qrsforever

if [[ $# != 1 ]]
then
echo "Error!: $0 m"
exit 0
fi

repo init \
         -u $git_host/manifests.git -b master \
         -m $1 \
         --repo-url=$git_host/git-repo.git \
         --repo-branch=stable \
         --no-clone-bundle
```

2. 0repoinit xxx.xml
