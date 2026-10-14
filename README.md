# 君居何位 · 测测你在唐朝能当什么官

一个**纯前端、零依赖、零后端**的唐代「结衔」生成器网页。

以八维心性测问（进取·权力·行事·价值·人际·知识·风险·忠诚）推演你在中晚唐官僚体系中的身份，
生成完整结衔（散官 → 检校官 → 宪衔 → 职事官 → 使职 → 勋官 → 爵位 → 食邑）、八维比例、
冠服图与逐层释义。

## 特点

- **单文件**：全部内容都在 `index.html` 里（内联 CSS / JS / 冠服图 SVG）。
- **无外部请求**：不加载任何 CDN、字体或接口，可离线双击打开。
- **移动端适配**：响应式，手机浏览器可直接玩。
- 进度用 `localStorage` 保存在本地，中断可续。

## 本地运行

直接双击 `index.html` 即可；

或起个本地服务器：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000/
```

## 部署到 GitHub Pages

1. 新建一个空仓库（例如 `junjuhewei`），把本目录推上去：

   ```bash
   git remote add origin https://github.com/<你的用户名>/<仓库名>.git
   git branch -M main
   git push -u origin main
   ```

2. 打开仓库 **Settings → Pages**：
   - **Source** 选 `Deploy from a branch`
   - **Branch** 选 `main`，目录选 `/ (root)`
   - 点 **Save**

3. 等约 1 分钟，访问：

   ```
   https://<你的用户名>.github.io/<仓库名>/
   ```

   这就是可以转发给任何人的链接。
