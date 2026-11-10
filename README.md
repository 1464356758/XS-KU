# XS-KU 小说参考库 · V4.6

原始小说保留原路径。新书正文放在独立仓库；本库提供按问题检索、原文阅读、拆书教材与迁移练习。

## 已处理范围

- 原文快照：90dbe70eec0ffd89b75bf98705bb402fbc6d6b54。
- 171份原文，541198341字节；按文件名书名与作者分168组，含31份无后缀文件。
- 74608个网页阅读单元，逐单元保留规范哈希及原始位置；阅读单元不等于核实后的章节。
- 实际阅读6本的开篇共9单元，形成12条有引文依据的教材；其余待按任务阅读。
- 1次已见参考的原创迁移练习及模型复盘，未做独立盲评或真实读者验证。

签约情况来自作者提供资料时的说明；具体平台与送审版本未核实。题材提示按文件名推断，已读样本另行标注。

## 开始使用

阅读[启动小说库.txt](启动小说库.txt)与[XS-KU接入与创作](docs/XS-KU接入与创作.md)。已有目录是catalog.json；教材在studies，练习在practices，复盘在reviews。新上传文件放根目录或incoming，先提交原文，再同步目录。

```bash
python3 tools/novel_library.py --root . catalog
python3 tools/novel_library.py --root . search --query "关系 主动选择"
python3 tools/novel_library.py --root . read --book 实际编号 --chapter 实际单元序号
python3 tools/novel_library.py --root . sync --repository-url https://github.com/1464356758/XS-KU
```

导出的参考摘要只带学习结论和回查位置。新书每章使用正式任务书记录本书用法，写后结合正文检查，按实际反馈继续修正。

## V4.6接线完成

新书模板与五个交付包的可复现源码位于[系统仓库](https://github.com/1464356758/xiaoshuoV5/tree/main/system_templates/v4.6)。本库保留全部原文与已有阅读记录；工具已补平台待核样本标记、同书候选去重，以及在线导出时的真实提交与原文校验。新书写后在原release报告核对教材实际效果及当前章证据。
