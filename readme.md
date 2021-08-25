
```



 使用方法：

 git clone git@github.com:91xcode/bash-utils.git

 sh test_mac_sun.sh




注意

#!/bin/bash
RED="\e[31m"
GREEN="\e[32m"
echo -e "h${RED}el${GREEN}lo";

To Mac 用户：在你的 Mac 终端上执行以上代码，可能会出现没效果的情况……我也入坑半天才发现，原来 Mac 的 Bash 是不支持 -e 参数的……（通过 man echo 得知）

知道原因这问题也就好解决了，如果想让 Mac 终端支持颜色字符，最简单的方法就是把 bash 换了。比如换成 zsh（再加上惊为天人的 oh-my-zsh 多棒！这个时候如果是写脚本记得把第一行改成 #!/bin/zsh）。但如果你不想换，或者你写脚本时依然用的是 #!/bin/bash，那么你还有一种选择就是用 printf 代替 echo






其他

curl https://raw.githubusercontent.com/91xcode/bash-utils/master/utils.sh > utils.sh && curl https://raw.githubusercontent.com/91xcode/bash-utils/master/template.sh > run.sh


然后参考 test_run.sh

```
