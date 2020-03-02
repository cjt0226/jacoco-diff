# jacoco-diff
在 jacoco 覆盖率报告的基础上，计算出增量覆盖率

蓝色钻石标志为增量代码


# 用法
```shell
# 使用本工具，计算增量覆盖率，并修改覆盖率报告
python main.py -d report_dir -o HEAD~1
```

## 参数说明
  \-h, \-\-help        打印帮助信息
  
  \-d, \-dir           工程目录
  
  \-o, \-old_version   指定对比的版本号, 如果该参数没有给出，默认与前一个版本进行对比(HEAD\~1)。该参数支持 git commit hash 或者 HEAD~n 的格式。
  
  \-r, \-report        Jacoco Report目录
  