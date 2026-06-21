# Uecook Sans

一款专为博客阅读设计的合成字体。  
中文采用开源 **思源黑体（Source Han Sans CN）** 的 GBK 子集，西文与数字替换为 **Google Sans Flex**（实例化为 opsz=80 / wght=500），经 fontTools 脚本合并为单一字体文件后，依据 OFL 1.1 协议以 **Uecook Sans** 发布。

---

## 一、字体组成

| 部分 | 来源 | 处理 | 许可证 |
|------|------|------|--------|
| 汉字 + 中文标点 | [思源黑体 CN](https://github.com/adobe-fonts/source-han-sans) | GBK 子集（约 2.1 万汉字），CFF（PostScript）轮廓转 TrueType | SIL Open Font License 1.1 |
| 西文 + 数字 + 拉丁补充 | [Google Sans Flex](https://fonts.google.com/specimen/Google+Sans+Flex) | 可变字体实例化（opsz=80, wght=500），upem 2000→1000 缩放，复合字形递归展平 | SIL Open Font License 1.1 |

合并后单文件：**Uecook_Sans_GBK.woff2**（约 3.49 MB，22739 字形，upem 1000，font-weight 500 / Medium）

---

## 二、设计动机

搭建个人博客时，希望找到一款既支持中文、又拥有漂亮西文字形的免费字体。  
- 最初尝试 **Mi Sans**、**HarmonyOS Sans**、**OPPO Sans**，但因许可证限制（禁止网页内嵌或需商业授权），无法在博客中自由使用。  
- 退而选择 **思源黑体**（OFL 协议，完全自由嵌入），但原生西文部分略显生硬，数字与英文不够现代。  
- 于是将 **Google Sans Flex** 的西文与数字移植过来，形成“中西合璧”的混搭字体。  

根据 OFL 1.1 协议规定，修改后的衍生作品不得使用原字体的保留名称（Reserved Font Name），因此新命名为 Uecook Sans。

---

## 三、获取与使用

### 下载
本仓库 [Releases](../../releases) 页面提供 `UecookSans.woff2` 文件。

### 在网页中嵌入（CSS）
```css
@font-face {
  font-family: 'Uecook Sans';
  src: url('/fonts/UecookSans.woff2') format('woff2');
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}
body {
  font-family: 'Uecook Sans', 'PingFang SC', 'Microsoft YaHei', sans-serif;
}
```

---

## 四、致谢

- [Adobe](https://github.com/adobe-fonts/source-han-sans) 开发的思源黑体
- Google 团队设计的 Google Sans 家族（OFL 版本）
- [FontTools](https://github.com/fonttools/fonttools) 提供的强大字体编辑能力
