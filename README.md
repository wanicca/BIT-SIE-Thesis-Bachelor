# BIT-Thesis-bachelor v0.1

# 北京理工大学本科毕业设计（论文）Latex模板（非官方）

**【注意！！！】本模板不具有官方效力，仅供学习交流使用。使用该模板意味着使用者对latex已有基本了解，并对使用latex模板进行论文写作可能带来的后果有所预期，作者不负责因为使用本模板而产生的损失与非技术问题。**

本模板基于[北京理工大学硕士（博士）学位论文LaTeX模板](https://github.com/BIT-thesis/LaTeX-template)修改实现，遵守学校的官方文件*【1书写规范】本科生毕业设计（论文）书写规范及打印装订要求 (新)_2018.6.12.doc*中指定的格式标准，对于该文件中未清楚声明的部分，作者进一步参考了*【2参考模板】参考论文示样.doc*中的表现效果。

latex模板可以使得使用者专注于内容而非格式，便捷地实现图表公式的编号及引用，自动生成良好的排版效果。使用教程可以参考[北京理工大学硕士（博士）学位论文LaTeX模板](https://github.com/BIT-thesis/LaTeX-template)中给出的资料和文件夹下的demo.tex样例。作者本人推荐使用Texlive套件+TexStudio进行撰写、编译、预览，编译器采用XeLatex。

由于原来研究生学位论文的latex模板和本科毕设书写规范要求有一定差别，本模板使用了单独的模板文件BIT-thesis-grd-bachelor.cls，无法再进行研究生学位论文的编译；此外，为了严格统一规范字体，力图与Word样例产生相同的效果，在本模板中规定死了字体使用微软字体，并使用伪粗体、伪斜体作为`\bf`等指令的效果，非windows用户需要手动添加windows字体到系统字库路径。

本模板相对参考目标，具体修改如下：

- 修改了标题字体，严格遵守宋体加粗标准，并单独创建了ctex-fontset-windowsfake.def来约束ctex字符集为windows字库，规定用伪粗体实现宋体加粗。
- 修改了页眉内容、字号、字间距0.5磅。
- 修改了页边距、页眉、页脚位置，尽量与规范要求及Word模板保持一致。
- 修改了正文字距，包括中文、英文字距0.5磅。
- 修改了各部分组织顺序，按照规范要求的摘要-目录-正文-致谢-参考文献-附录顺序组织，由于这种顺序，附录放在了\backmatter之后，因此无法再像研究生模板一样区分附录A、B，附录标题需要在附录章节手动指定。
- 修改了目录缩进、加粗策略，与规范要求、参考论文样式进行统一；去掉了目录中的摘要部分。
- 修改了摘要的关键字，保留了“关键词”之前的缩进，与参考论文样式一致。
- 修改了列表行距，使得与参考论文的效果大致相同（但在缩进策略上，暂时采取了和正文首行一样缩进2字符，而不是像参考论文里的那种难以描述的效果）。

除此之外，由于编号策略与引用格式硕博学位论文要求一致，没有进行修改。最终效果可以参考*模板编译效果.pdf*。

目前的版本可能存在的问题：

- 作者仍未搞清标题段落间距换算关系，尽管通过目测对比调整多次，但仍然可能与参考论文的效果不精确相等，此外页眉位置也可能未必精确相同。
- 由于字距调整方式与word不一样，也需要经过换算，并且中文、英文需要分别调整，因此可能数值上没有达到精确与word相同，但基本效果一致，编译可以达到和*【2参考模板】参考论文示样.doc*相近效果。由于word排版不佳的缘故，参考论文里一些地方产生的换行未必合理，导致页面参差不齐，对于这种情况，作者没有追求与word参考论文完全相同。
- 图表位置会自动浮动到合适位置，有可能与word插图位置不一样，这是latex使用的正常现象。
- 本版本不包括摘要之前的内容（如封面），因为制作本模板时学校还未发布相关文件。后期视情况加入，有可能需要使用者另外打印。
- 目录部分未规定字间距，这里按照正文要求进行了设置。
- 无序列表的点号采用了$\bullet$，没有和word完全一致，无序列表的缩进也与word参考没有保持一致（作者认为没必要）。
- ...

最后，目前版本只是初步尝试，可能还存在很多没有发现的问题；作者本人也是latex菜鸟，姿势水平不够，因此欢迎各位试用，并讨论模板使用中的相关技术问题与解决方案。



## 感谢

感谢[北京理工大学硕士（博士）学位论文LaTeX模板](https://github.com/BIT-thesis/LaTeX-template)的作者们。