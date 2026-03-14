# 🔮 电子水母 - 数学公式生成动画

一个使用纯数学公式生成的电子水母动画，支持交互式参数调整。

![电子水母预览](preview.gif)

## 在线演示

访问 GitHub Pages: https://yourusername.github.io/jellyfish/

## 功能特点

- 🎨 使用纯数学公式生成水母形态
- 🎬 实时动画预览
- ⚙️ 6个可调参数
- 💾 支持下载动画

## 参数说明

| 参数 | 说明 | 范围 |
|------|------|------|
| 游动速度 | 水母游动速度 | 0.02 - 0.5 |
| 水母密度 | 粒子数量 | 5000 - 50000 |
| 粒子大小 | 点的大小 | 0.1 - 2.0 |
| 尾部/触手长度 | 触手长度 | 40 - 180 |
| 触手摆动幅度 | 波动幅度 | 0.3 - 4.0 |
| 触手摆动频率 | 波动频率 | 0.5 - 6.0 |

## 数学公式

```
k = 5 * cos(x/14) * cos(y/30)
e = y/8 - 13
d = (k² + e²)/59 + 4
a = atan2(k, e)
q = 60 - sin(a*e) + k * (3 + (4/d) * sin(d² - 2t))
c = d/2 + e/99 - t/18
X = q * sin(c) + 200
Y = (q + 9d) * cos(c) + 200
```

## 本地运行

直接在浏览器中打开 `index.html` 文件即可。

## 技术栈

- HTML5 Canvas
- JavaScript (原生)
- 数学公式生成

## 部署到 GitHub Pages

1. 创建 GitHub 仓库
2. 上传 `index.html` 文件
3. 进入 Settings → Pages
4. Source 选择 `main` 分支
5. 保存后访问生成的链接

## 参考

原始公式来源: https://xiabanglu.github.io/jellyfish/
