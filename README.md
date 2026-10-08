# STUDIO (WXZ) — Photography Studio Official Site

黑白双 logo 的摄影工作室官网。设计语言参考 Apple iPhone 产品页：黑色舞台、巨幅 Raleway 字重对比、滚动驱动的视差与 sticky 缩放叙事，移动端同样保持完整动效。

## Structure

```
index.html          # 单文件站点（内联 CSS/JS，无 build）
assets/logo/        # STUDIO (WXZ) 黑白 logo
assets/img/         # AI 生成的摄影风格视觉素材（已裁水印、压缩）
```

## Scroll Effects（原生 JS + rAF，无外部库）

1. Hero 背景双层视差 + 文案上浮淡出
2. Apple 标志性 sticky 缩放章节：小卡片随滚动放大至全屏
3. 图文行反向视差（图片在遮罩内以不同速度位移）
4. 垂直滚动驱动的横向作品画廊（sticky + translate3d）
5. IntersectionObserver 入场 reveal、导航毛玻璃 scrim
6. `prefers-reduced-motion` 全量降级为静态布局

## Typography

Raleway（Google Fonts，200/700/800 字重对比）+ 系统中文回退。

© STUDIO (WXZ)
