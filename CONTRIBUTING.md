# 贡献指南

欢迎贡献代码、文档，或提交 Issue！让我们一起把这个项目做得更好。

## 🚀 如何开始

1. **Fork 本仓库**
2. **Clone 到本地**
   ```bash
   git clone https://github.com/yourusername/contract-ai-pro.git
   cd contract-ai-pro
   ```
3. **创建你的 Feature 分支**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
4. **提交你的改动**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
5. **推送到分支**
   ```bash
   git push origin feature/AmazingFeature
   ```
6. **开启一个 Pull Request**

---

## 📝 可以贡献什么

### 1. 新增风险规则
在 `scripts/review_contract.py` 的 `RISK_RULES` 列表中添加新的规则：

```python
{
    "id": "R009",
    "name": "风险名称",
    "level": "high",  # high/medium/low
    "category": "分类",
    "patterns": [r"正则表达式1", r"正则表达式2"],
    "risk": "风险说明",
    "suggestion": "修改建议",
    "law_ref": "法律依据"
}
```

### 2. 新增合同模板
在 `scripts/generate_contract.py` 的 `CONTRACT_TEMPLATES` 字典中添加新模板：

```python
"新模板名称": {
    "name": "模板显示名称",
    "description": "模板说明",
    "template": """模板内容，使用{变量名}占位""",
    "required_fields": ["变量1", "变量2", ...]
}
```

### 3. 修复 Bug
发现 Bug 请先提交 Issue，再提交 PR 修复。

### 4. 完善文档
- 优化 README
- 补充使用教程
- 翻译多语言版本
- 补充示例合同

### 5. 功能开发
查看 [开发计划](#开发计划)，选择你感兴趣的功能开发。

---

## 🎯 开发计划

### v1.1 版本（进行中）
- [ ] 增加PDF文件解析支持
- [ ] 增加Word文档解析
- [ ] 增加更多合同类型模板
- [ ] 优化风险规则库（增加到20+条规则）

### v1.2 版本
- [ ] 接入大模型API做深度语义分析
- [ ] 支持批量审查多个合同
- [ ] 增加合同对比功能
- [ ] 支持导出PDF格式报告

### v2.0 版本
- [ ] Web界面版本
- [ ] 用户账号系统
- [ ] 合同历史管理
- [ ] 团队协作功能
- [ ] API接口

---

## 📋 Pull Request 规范

### 提交前检查
- [ ] 代码风格保持一致
- [ ] 测试所有功能正常运行
- [ ] 更新相关文档
- [ ] 提交信息清晰描述改动

### 提交信息格式
```
<类型>: <描述>

例如：
feat: 增加租赁合同模板
fix: 修复重复识别问题
docs: 更新README使用说明
refactor: 重构风险识别逻辑
```

### 类型说明
- `feat`: 新功能
- `fix`: 修复Bug
- `docs`: 文档更新
- `style`: 代码格式调整
- `refactor`: 重构（既不是新增功能，也不是修复Bug）
- `test`: 测试相关
- `chore`: 构建过程或辅助工具的变动

---

## 🐛 提交 Issue

### Bug 反馈
请包含以下信息：
1. **复现步骤**：如何复现这个问题
2. **期望行为**：你期望发生什么
3. **实际行为**：实际发生了什么
4. **环境信息**：Python版本、操作系统等
5. **错误日志**：如有报错，请附上完整日志

### 功能建议
请描述清楚：
1. **这个功能解决什么问题**
2. **你期望的实现方式**
3. **有没有类似的产品参考**

---

## 💬 行为准则

- 保持友好和尊重
- 接受建设性的批评
- 聚焦于对项目最有利的事情
- 对社区其他成员友善

---

## 📞 联系我们

- 提交 Issue：[GitHub Issues](https://github.com/yourusername/contract-ai-pro/issues)
- 邮件：your@email.com

---

**感谢所有为这个项目做出贡献的人！** 🙏

<a href="https://github.com/yourusername/contract-ai-pro/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=yourusername/contract-ai-pro" />
</a>
