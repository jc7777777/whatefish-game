# WorkBuddy 工作记忆

## 用户信息
- 用户名：baojuansheng
- GitHub 账号：jc7777777

## 项目信息
### 《你什么鱼》游戏
- 位置：/Users/baojuansheng/WorkBuddy/Claw/
- 游戏文件：
  - sheep_game.html（原始版本）
  - sheep_game_with_bg.html（背景图嵌入版本）
  - BG.jpg（背景图）
- GitHub Pages 链接：https://jc7777777.github.io/whatefish-game/
- 仓库地址：https://github.com/jc7777777/whatefish-game
- 卡牌排版：每行5列，间距 68（横）×62（纵），第二关及以后左移7px
- 卡槽区：2×2田字形排列，固定高度233px，宽度70%居中，卡牌直接撑满格子（不用scale）
- 卡牌区宽度：105%（两侧各延伸2.5%）
- 槽满无法消除直接判定失败（不返还卡牌）
- 槽位卡牌选中后不显示边框和背景
- 背景音乐：Web Audio API 合成 City Pop × Jazz × Dante Peluso 风格循环BGM（BPM=98，音量0.045）
  - 结构：Rhodes旋律+Lead吉他叠层 + 爵士和弦pad(Cmaj9/Am11/Dm9/G13) + 稀疏切音comping + Jazz Walking Bass + Ride cymbal主导爵士鼓组
  - 和弦进行：Cmaj9 → Am11 → Dm9 → G13（II-V-I 爵士变体，每4拍换一次）
  - Dante Peluso 元素：playLeadGuitar()、playSlide()、旋律 C5→A5 六度钩子
  - 旋律爵士元素：切分提前落拍、b7蓝调音(G4)、句子间留白
  - 贝斯：Walking bass（正弦+三角波叠加，upright bass 质感），每拍行走
  - 鼓组：ride 每拍滴答、轻 kick、刷式 snare、偶尔 rim/closed hihat ghost note
  - 循环间隔：每段结束后静默 1.3 秒再循环
  - 游戏开始后延迟 1.5 秒进入BGM
