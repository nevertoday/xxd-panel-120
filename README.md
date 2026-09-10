# XXD Panel 120｜建筑概念手绘志

把照片中的空间记忆，变成留白充分的建筑概念草图。

[简体中文](README.md) · [English](README.en.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [العربية](README.ar.md)

## 样张展示

本项目已发布 8 张实际样片，图片文件位于 `assets/examples/`。

| sample-05 | sample-06 |
| --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 适用场景与解决的问题

想把照片变成有设计推敲感的概念图，却不希望得到一张逐物描摹的完整场景？Panel 120 保留照片的身份与空间记忆，把核心形体、轮廓和关系提炼成自由徒手透视线稿。少量色块、几何辅助线和大面积留白共同构成作品。

### 适合这些情况

- 建筑、空间、旅行或物件照片需要转成有编辑气质的概念手绘。
- 原图构图弱、背景杂、主体小，希望通过删减、重组和尺度变化重新组织视觉重点。
- 希望保留识别度与空间关系，同时避免满幅上色或写实效果图。
- 同一风格需要上下、左右、纯设计、壁纸和目录批量交付。

### 它替你解决什么

- 删除背景和次要物件，留下代表主题的核心形体与视觉记忆点。
- 使用放松、克制、稍有反复的透视线和少量构造线表达设计探索。
- 把留白纳入构图，避免以装饰或色块填满画面。
- 对照图严格只有两个等分区域；每张原图独立生成，避免二次风格化。

## 原始提示词 · 五种语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中文逐字保存用户原文，是运行时唯一创作与审美权威；其余版本为完整忠实的阅读译文。

建筑概念透视草图 · 徒手线稿 · 几何参考线 · 少量色块和阴影 · 2–4 色照片取色 · 超大量留白 · 极少量编辑注记

## 它如何把照片变成成品

识别主题与空间关系 → 提炼核心形体 → 删除复杂背景 → 重组尺度与裁切 → 以透视线、几何辅助线和少量色块重构 → 用大量留白和短注记完成

## 成品中最容易识别的特点

- 上方或左侧保留真实照片，仅轻微调色，不改变主体身份和姿态。
- 设计区是建筑概念手绘，而非完整场景描摹、写实效果图或 3D。
- 主体精炼且较小，可偏心、贴边、局部裁切，余白主动参与构图。
- 2–4 种原图颜色整理为干净、克制的色系，只在重点部位轻铺。
- 几何阴影表现体量与进深，少量辅助线保留设计推敲感。
- 极少量文字安静置于留白，不限定字体模板；样张采用英文。

所选交付模式只映射布局，不改变原文审美：`left-right` 将原文上方照片移至左侧、下方设计移至右侧；所选比例覆盖原文默认 `3:4`。

## 四种输出模式

- `top-bottom`：整张画布只有上下两个全宽区域，现实照片在上、设计在下，严格各占 50%。
- `left-right`：整张画布只有左右两个全高区域，现实照片在左、设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现 Panel 120 的设计转译，照片只作为不可见参考。
- `wallpaper-pack`：按手机、iPad、桌面和手表分别生成完整设计壁纸，可选 `linked` 连贯套装或 `independent` 四张独立。

支持多选模式与比例（`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5` 或准确像素），以及模型生成文字、准确文字和无文字。传入目录会递归扫描图片，每张源图独立处理，共用一次交付设置；最终 PNG 平铺放入一个新任务目录。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-120.git
npx skills add https://github.com/nevertoday/xxd-panel-120 --skill xxd-panel-120
```

安装后重新启动 Agent 会话，然后调用 `$xxd-panel-120`。也可以按需追加 `--global --agent codex --yes` 做用户级安装。

常用调用示例：

```text
/xxd-panel-120 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale zh-CN
/xxd-panel-120 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-120 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-120 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完整运行契约见 [SKILL.md](SKILL.md)；运行适配器见 [英文](references/xxd-panel-120-prompt.en.md) 与 [中文](references/xxd-panel-120-prompt.zh-CN.md)。

<!-- xxd-readme-ads:start -->
## 关于 XXD

XXD 是小小东品牌名的缩写，本项目由小小东创建并维护： [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## 广告信息｜XXD 付费服务与会员

> **广告与商业信息声明：** 以下二维码、会员与付费服务链接属于小小东的广告信息。是否扫码或购买完全自愿，不影响本开源项目的访问与使用。


<!-- xxd-panel-command-system:start -->

将军 Skills 已包含在 699 元/年的统一会员权益中，无需单独购买。

| 层级 | Skill | 负责什么 |
|---|---|---|
| **将军级** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 识别当前可用的编号 Skills；按图片、主题和用途推荐；按编号点将；组织同图多风格试稿；为图片文件夹批量分配并逐项派发。 |
| **士兵级** | `xxd-panel-NNN` | 每个编号只执行自己独立的原始提示词与审美，把将军派发的单个任务完成为成品。 |

<!-- xxd-panel-command-system:end -->

### 知识星球＋成员提示词库＋Skills 所有将军会员 · 699 元/年

[知识星球](https://wx.zsxq.com/group/15554814142882)、[小小东成员提示词库](https://vip.xiaoxiaodong.ai/)与 Skills 所有将军会员是同一份会员权益：**一次年费同时开通三项权益，无需重复付费。**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 许可证

本项目（包括 Skill、提示词、脚本、文档及随附样张）采用 **PolyForm Noncommercial License 1.0.0**。完整法律条文请见 [LICENSE](LICENSE)，官方页面见 <https://polyformproject.org/licenses/noncommercial/1.0.0>。

用人话说：

- 个人可以用于学习、研究、实验、测试、兴趣项目和私人娱乐；慈善机构、教育机构、公共研究/安全/卫生机构、环保组织及政府机构也可以使用。
- 在**非商业目的**下，你可以使用、复制、修改、制作衍生作品并分享；分享时必须同时提供本许可证（或上面的链接）以及作者提供的所有 `Required Notice:` 声明。
- 不允许用于商业产品或服务、收费交付、出售访问权或许可，或任何预期会带来商业应用的用途。需要商业使用时，请先向版权方另行取得书面许可。
- 本协议只授予其中明确写出的著作权许可和有限的专利许可，不授予商标、品牌名称或其他未明确授予的权利，也不能把你的许可再转授给他人。
- 如果收到书面违约通知，须在 32 天内纠正并采取实际补救措施，否则许可会立即终止；就专利侵权提出书面主张也会终止专利许可。
- 内容按“现状”提供，在法律允许的范围内不作任何担保，使用风险和可能的损失由使用者自行承担。
