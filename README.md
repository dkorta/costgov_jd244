# costgov_jd244

**统计成本与容量治理专家·检索召回的漏斗分析各部分的长度占比并标出异常。**

`costgov_jd244` —— 按段落统计成本与容量治理专家·检索召回的漏斗分析相关的长度分布，标出过长、过短与重复表达的部分

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`costgov_jd244.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**阿里巴巴 · 专家成本与容量治理专家**
- 技能主线：大模型推理、Kubernetes、LLM评测
- 领域标签：AI基础设施
- 研究方向：成本与容量治理专家·检索召回的漏斗分析

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install dkorta-costgov_jd244
```

装完直接用命令名调用：

```bash
costgov_jd244 --help
```

也可以不用安装，直接把 `costgov_jd244.py` 拷走用——它只依赖标准库。

## 为什么需要它

区分「重复」与「必要冗余」——后者是刻意强调，不计入冗余

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python costgov_jd244.py --file input.txt
python costgov_jd244.py --text "示例内容"
python costgov_jd244.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 长度按字符与词统计，与具体 tokenizer 有偏差。
- 不判断长度是否「合理」，只报告分布。

## 跑测试

```bash
python test_costgov_jd244.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/dkorta/costgov_jd244>

---

## 关于作者

dkorta 做成本与容量治理专家·检索召回的漏斗分析相关的问题，方向对标阿里巴巴的专家成本与容量治理专家岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://dkorta.github.io>
- 仓库：<https://github.com/dkorta/costgov_jd244>

## 许可

MIT，见 [LICENSE](LICENSE)。
