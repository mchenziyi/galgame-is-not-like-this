# 旮旯给木里不是这样的

> Galgame 不是这样的。

一个运行在 [Reasonix](https://github.com/reasonix/reasonix) 上的**视觉小说世界引擎** skill。

谁不想在公司摸鱼的时候来一场甜甜的恋爱呢。

## 你能获得什么

一个真正活着的故事。

这里的 NPC 不会在你出现时才苏醒——他们有自己的人生。你离开的每一天，世界都在继续：邻居可能在某个深夜做出了改变一生的决定，常去的咖啡馆可能悄悄换了老板，而你两周前在走廊里偶然听到的那句话，会在未来的某一天突然拼进拼图的缺口。

没有强制的剧情高潮，没有围绕你公转的角色。你只是一个恰好住在这栋老旧公寓里的普通人。当你开始珍惜那些平凡的日常时，故事才真正开始。

## 核心理念

- 世界有自己的运转逻辑，不围着玩家转
- NPC 拥有独立的人生、目标和秘密
- 玩家缺席时世界继续推进——离屏事件真实发生
- 日常比高潮更重要；羁绊比离别更珍贵

```
世界一致性 > 角色一致性 > 因果逻辑 > 叙事节奏 > 玩家意愿
```

## 安装

```bash
# 在 Reasonix 项目目录下
reasonix install-skill https://github.com/mchenziyi/galgame-is-not-like-this/blob/master/旮旯给木里不是这样的.md
```

或者直接把 `旮旯给木里不是这样的.md` 复制到项目的 `.reasonix/skills/galgame_world_engine/SKILL.md`。

## 运行

```
/galgame_world_engine
```

引擎会从 `.game/` 读取存档并恢复世界状态。首次运行自动初始化默认世界。

## 文件结构

| 文件 | 说明 |
|------|------|
| `旮旯给木里不是这样的.md` | 引擎定义（skill 源文件） |
| `.reasonix/skills/galgame_world_engine/SKILL.md` | 安装后的 skill |
| `.game/world.json` | 实体图谱 + 关系 |
| `.game/characters.json` | 角色档案 + 关系数值 |
| `.game/story.json` | 故事进度 + 叙事状态 |
| `.game/timeline.json` | 时间线 + 压缩历史 |

`.game/` 目录在 `.gitignore` 中——每个玩家的世界都是独一无二的，不该被版本控制。

## 许可证

MIT
