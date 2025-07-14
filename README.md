## **Actions_SukiSU_oppo_kernel_sm8475**
#####
**```Build SM8475 For OPPO Devices SukiSU Ultra Kernel```**
#####
**一个更方便、快捷的自动化 OPPO 系列骁龙 8+ Gen 1(SM8475)平台机型的通用内核编译脚本。**
#####
## **Tips:**
- **由于傻逼绿厂摆烂，开源的内核只他妈开源到一半，不学一加一样整个 manifest 合集，导致有些东西死活都编译不了，来来回回折腾大半天**
- **官方给开发人员使用的 Bazel 编译器过于逆天，而且效率跟吃了石一样慢，还容易出现各种莫名其妙的报错，编译将近一个小时结果你妈的血亏😭**
- **由于傻逼绿厂大规模魔改内核 f2fs，导致OPPO/一加/真我机型不清空 data 分区还进不去**
- **由于 Common Kernel Open Source 的缘故，本项目仅提供 OPPO SM8475 平台对 ColorOS 15 的支持**
#####
>[!IMPORTANT]
>- **关于 Actions 要跑多久，个人觉得用 clang+ccache 编译器跑的速度就快，实测跑完需要 19-35 分钟，最久可达 42 分钟，而官方给的 Bazel 编译器过于逆天，速度为 29-35 分钟，最久可达到将近一个小时，且容易血亏(指 Bazel 编译的时候报错)。**
>- **本项目不会提供 Bazel 编译方式，而是使用 clang+ccache 的编译方式**
#####
## **更新日志：**
- [x] **添加 KPM,VFS,ZRAM,Sufus 补丁的支持**
- [x] **添加对 OPPO Reno9 Pro Plus(OPPO Reno9 Pro+) 机型的编译**
- [x] **使用 clang+ccache 编译，速度更快**
- [x] **添加三星 SSG IO 调度器支持(来自@cctv18)**
- [x] **编译支持 BBR/Brutal 及一系列 TCP 拥塞控制算法**
- [x] **lz4 1.10.0 & zstd 1.5.7 算法更新 && 优化补丁(来自@ferstar,移植@Xiaomichael)**
#####
## **待完成功能：**
- [ ] **新增同 SM8475 机型的支持**
- [ ] **新增对 EROFS 文件系统的支持**
- [ ] **合并同 SM8475 机型为一个脚本编译**
- [ ] **更多的优化及特性**
#####
## **项目鸣谢:**
**项目的诞生离不开这些项目的贡献和支持：**
- SukiSU Ultra：[SukiSU-Ultra/SukiSU-Ultra](https://github.com/SukiSU-Ultra/SukiSU-Ultra)
- Susfs4ksu：[ShirkNeko/susfs4ksu](https://github.com/ShirkNeko/susfs4ksu)
- SukiSU_Patch：[SukiSU-Ultra/SukiSU_patch](https://github.com/SukiSU-Ultra/SukiSU_patch)
- GKI 内核构建脚本代码：[Numbersf/Action-Build](https://github.com/Numbersf/Action-Build)
- README 及部分 GKI 构建脚本代码:[cctv18/oppo_oplus_realme_sm8650](https://github.com/cctv18/oppo_oplus_realme_sm8650)
#####
**感谢以上大佬们对这些项目的付出!**
#####
## **项目所使用的 OPPO 开源内核：**
- **OPPO SM8475 Kernel Open Source开源地址：[oppo-source/android_kernel_oppo_sm8475](https://github.com/oppo-source/android_kernel_oppo_sm8475)**
- **OPPO SM8475 Common Kernel Open Source开源地址：[oppo-source/android_common_oppo_sm8475](https://github.com/oppo-source/android_common_oppo_sm8475)**
