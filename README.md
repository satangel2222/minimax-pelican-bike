# 🦢 minimax-m3.1-flash-free 骑自行车

纯原生 **SVG + CSS** 绘制的 2D 动画：模型 `minimax-m3.1-flash-free` 化身一只鹈鹕，骑着自行车在乡间公路上飞驰。

- 无任何依赖：无 canvas、无图片资源、无第三方库，单个 HTML 文件
- 车轮 / 曲柄 / 踏板 / 地面滚动速度严格一致（轮半径 60，0.8s/圈 → 471 px/s）
- 双腿由**二连杆逆运动学**解算，脚步始终贴合踏板，膝盖朝前
- 嵌套旋转使用显式 `matrix()` 指定旋转中心，规避 SVG `transform-origin` 在嵌套变换下的语义歧义
- 内置播放 / 暂停与 0.5×–2× 变速控制

## 在线观看

https://satangel2222.github.io/minimax-pelican-bike/

## 本地打开

直接双击 `index.html` 即可，无需服务器。

## 重新发布

```bash
cd publish
git add -A && git commit -m "update"
git push
```

GitHub Pages 会在几十秒内自动更新。
