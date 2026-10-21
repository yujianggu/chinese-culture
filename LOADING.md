# 按需加载约定

先读取根README及根catalog.json，沿`domains[].catalog`和`groups[].catalog`选择分类，再从主题摘要进入正文；相关链接不自动展开，不一次性读取全库。已知主题ID时用`python3 scripts/kb.py resolve <ID>`获取读取清单。

- `brief`：摘要；`detail`：摘要和正文；`examples`、`sources`、`assets`：选定主题及对应支撑入口。必需依赖`requires`按工具展开；相关推荐`related`不自动展开。
- `topic.json`的入口路径相对其所在目录；生成索引的路径相对本项目根目录，不允许越出本项目。
- 保留已发布的`culture.*`主题ID和正文路径。跨项目引用时固定本仓库Git提交，而非仅记录分支名。
- 实际应用时读取正文、适用边界及来源；古文、现代译文和教学借鉴分别标明。原义待核实的`reference`条目需要`--allow-reference`；`example`条目不作为企业事实或通用标准。
- `--max-bytes`限制读取清单的UTF-8字节数；超预算须缩小主题范围，不能省略必要依赖。
- 古籍采集记录、版本差异、缺文和译注覆盖范围沿用各书说明。迁移不构成事实或文本版本复核。
