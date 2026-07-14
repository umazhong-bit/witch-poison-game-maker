# 女巫的毒药游戏生成器

一个面向英语课堂的 Xiaoba CLI Skill。教师提供英语词汇后，它会生成可离线运行的“女巫的毒药”双组课堂认读游戏 HTML。

## 功能

- 5×5 词汇棋盘
- A、B 两组秘密设置毒药
- 教师控制“读对/读错”和课堂节奏
- 支持全屏课堂大屏
- 输出单文件 HTML，无需联网
- 同时生成记录词表与规则版本的 manifest 文件

## 使用方法

```bash
python3 scripts/generate_game.py \
  --words "museum, school, train station, shop, cinema, park, mountain, library" \
  --output "/目标目录/女巫的毒药.html"
```

详细工作流程和固定教学规则请参阅 [`SKILL.md`](SKILL.md)。

## 目录结构

```text
witch-poison-game-maker/
├── SKILL.md
├── agents/openai.yaml
├── assets/witch-poison-template.html
└── scripts/generate_game.py
```

