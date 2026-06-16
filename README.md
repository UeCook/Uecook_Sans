# Uecook_Sans

一款专为博客阅读与品牌展示设计的合成字体。  
中文采用开源 思源黑体（Source Han Sans），西文与数字替换为 Google Sans Flex，经手动合并与调优后，以 Uecook Sans 发布。

---

## 一、字体组成

| 部分 | 来源 | 许可证 |
|------|------|--------|
| 汉字（CJK） | [思源黑体](https://github.com/adobe-fonts/source-han-sans) | SIL Open Font License 1.1 |
| 西文 + 数字 | [Google Sans Flex](https://fonts.google.com/specimen/Google+Sans+Flex) | SIL Open Font License 1.1 |


---

## 二、设计动机

搭建个人博客时，希望找到一款既支持中文、又拥有漂亮西文字形的免费字体。  
- 最初尝试 **Mi Sans**、**HarmonyOS Sans**、**OPPO Sans**，但因许可证限制（禁止网页内嵌或需商业授权），无法在博客中自由使用。  
- 退而选择 **思源黑体**（OFL 协议，完全自由嵌入），但原生西文部分略显生硬，数字与英文不够现代。  
- 于是将 **Google Sans Flex** 的西文与数字移植过来，形成“中西合璧”的混搭字体。  

根据 OFL 1.1 协议规定，修改后的衍生作品不得使用原字体名称，因此新命名为 Uecook Sans。

---

## 三、获取与使用

### 下载
本仓库 [Releases](../../releases) 页面提供最新 `.ttf` / `.woff2` 文件。

### 在网页中嵌入（CSS）
```css
@font-face {
  font-family: 'Uecook Sans';
  src: url('/fonts/UecookSans.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}
body {
  font-family: 'Uecook Sans', 'PingFang SC', 'Microsoft YaHei', sans-serif;
}
```

### 本地安装
- Windows：双击 `.ttf` 文件，点击“安装”
- macOS：双击 `.ttf`，在“字体册”中安装
- Linux：复制到 `~/.local/share/fonts/` 并执行 `fc-cache -fv`



---

## 四、致谢

- [Adobe 与 Google](https://github.com/adobe-fonts/source-han-sans) 开发的思源黑体
- Google 团队设计的 Google Sans 家族（OFL 版本）
- [FontTools](https://github.com/fonttools/fonttools) 提供的强大字体编辑能力

