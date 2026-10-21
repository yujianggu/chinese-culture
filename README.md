# Chinese Culture · 中国瑰宝

中华历史、佛家、道家、儒家及经典原文的独立知识库，迁自 `yujianggu/kb` 的“中国瑰宝”目录。目录结构、已发布的 `culture.*` 主题ID及正文路径保持不变；内容来源、原义待核实及教学示例标记继续沿用。

## 阅读入口

- [中国瑰宝总览](中国瑰宝/README.md)
- [文化分层索引](中国瑰宝/catalog.json)
- [中华历史](中国瑰宝/中华历史/README.md)
- [经典原文](中国瑰宝/经典原文/README.md)
- [按需加载约定](LOADING.md)
- [结构维护](CONTRIBUTING.md)

先读取本页与加载约定，按领域、分类、主题摘要逐级选取内容，不一次性读取全部正文。实际使用方法或解释原文时读取适用边界与来源说明。

## 索引工具

在本项目根目录执行（Python 3.9及以上，无第三方依赖）：

```bash
python3 scripts/kb.py resolve culture.classics.lunyu --layer brief
python3 scripts/kb.py resolve culture.classics.shiji --layer detail
python3 scripts/kb.py build
python3 scripts/kb.py check
```

`catalog.json`和`index/topics.json`由工具生成，不手工编辑。迁移时仅调整导航和索引归属，未重新核验正文事实、古籍版本或翻译覆盖范围。

[通用知识库](https://github.com/yujianggu/kb)
