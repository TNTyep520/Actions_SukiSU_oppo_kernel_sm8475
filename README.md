# **Actions_SukiSU_oppo_kernel_sm8475**
#####
**```Build SM8475 For OPPO Devices SukiSU Ultra Kernel```**
#####
**一个更方便、快捷的自动化 OPPO 系列骁龙 8+ Gen 1(SM8475)平台机型的通用内核编译脚本。**
#####
# **Tips:**
- **由于傻逼绿厂摆烂，开源的内核只他妈开源到一半，不学一加一样整个 manifest 合集，导致有些东西死活都编译不了，来来回回折腾大半天**
- **官方给开发人员使用的 Bazel 编译器过于逆天，而且效率跟吃了石一样慢，还容易出现各种莫名其妙的报错，编译将近一个小时结果你妈的血亏😭**
- **由于傻逼绿厂大规模魔改内核 f2fs，导致OPPO/一加/真我机型不清空 data 分区还进不去**
#####
>[!IMPORTANT]
>- **关于 Actions 要跑多久，用 clang+ccache 的方式跑的速度就快，实测大部分机型跑完需要 19-35 分钟，最久 42 分钟而官方给的 Bazel 编译器速度为 29-35 分钟，最久可达到将近一个小时。**
>- **本项目不会提供 Bazel 编译方式，而是使用 clang+ccache 的方式**
#####
# **项目鸣谢**：
- SukiSU Ultra：[SukiSU-Ultra/SukiSU-Ultra](https://github.com/SukiSU-Ultra/SukiSU-Ultra)
- Susfs4ksu：[ShirkNeko/susfs4ksu](https://github.com/ShirkNeko/susfs4ksu)
- SukiSU_Patch：[SukiSU-Ultra/SukiSU_patch](https://github.com/SukiSU-Ultra/SukiSU_patch)
- GKI 内核构建脚本代码：[Numbersf/Action-Build](https://github.com/Numbersf/Action-Build)
- README 及部分 GKI 构建脚本代码:[cctv18/oppo_oplus_realme_sm8650](https://github.com/
cctv18/oppo_oplus_realme_sm8650)
#####
**感谢以上佬们对这些项目的付出!**
#####
# 附本项目中所使用的 OPPO 内核开源地址：
- **OPPO SM8475 Kernel Open Source开源地址：[oppo-source/android_kernel_oppo_sm8475](https://github.com/oppo-source/android_kernel_oppo_sm8475)**
- **OPPO SM8475 Common Kernel Open Source开源地址：[oppo-source/android_common_oppo_sm8475](https://github.com/oppo-source/android_common_oppo_sm8475)**