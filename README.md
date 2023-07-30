<!--
 *  =======================================================================
 *  ····Y88b···d88P················888b·····d888·d8b·······················
 *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
 *  ······Y88o88P··················88888b·d88888···························
 *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
 *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
 *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
 *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
 *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
 *  ·······························································888·····
 *  ··························································Y8b·d88P·····
 *  ···························································"Y88P"······
 *  =======================================================================
 * 
 *  -----------------------------------------------------------------------
 * Author       : 焱铭
 * Date         : 2023-07-01 16:06:50 +0800
 * LastEditTime : 2023-07-30 16:23:37 +0800
 * Github       : https://github.com/YanMing-lxb/
 * FilePath     : \SCI-LaTeX-Submission-Process-for-Elsevier\README.md
 * Description  : 
 *  -----------------------------------------------------------------------
 -->

# SCI-LaTeX-Submission-Process-for-Elsevier

## 介绍
自制的爱斯维尔期刊的LaTeX投稿工作流程模板

## 工作流程
### Manuscript-CN
### Manuscript-EN
### Revision-Major
### Revision-Minor
### Accepted-Manuscript
### Final Manuscript

### 本地部署写作

1. 编译该模板中文请使用 XeLaTeX或LuaLaTeX 引擎，英文可选用PdfLaTeX。

2. 本地部署LaTeX环境请转到[YM VSCode Configurations for LaTeX](https://github.com/YanMing-lxb/YM-VSCode-Configurations-for-LaTeX)项目

## 技巧
1. 提高编译速度
    - 在`documentclass`命令之前根据编译器的不同输入以下对应的命令
        - \special{dvipdfmx:config z 0} % XeLaTeX 取消PDF压缩，加快编译速度
        - \pdfcompresslevel=0 % PdfLaTeX 取消PDF压缩，加快编译速度
        - \pdfobjcompresslevel=0 % LuaLaTeX 取消PDF压缩，加快编译速度
    - EN-Manuscript.tex 使用 PDFLaTeX 编译

## 注意
1. abstract 和 keyword 环境中的内容不要为空，否则参考文献引用不会显示
2. CN-Manuscript.tex 使用 XeLaTeX 或 LuaLaTeX 编译均可
3. EN-Manuscript.tex 使用 PDFLaTex、XeLaTeX 与 LuaLaTeX 均可，但 PDFLaTex 编译最快
4. 有时会存在在1-Manuscript-CN文件夹中的tex文件中编译时，编译成EN-Manuscript.tex的情况，发生此问题时，只需在CN-Manuscript.tex中编译一下即可


## 参与贡献
