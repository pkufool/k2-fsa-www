---
title: Sherpa Onnx 常见问题
date: 2024-11-08
categories:
  - FAQ
comments: true
authors:
  - pkufool
slug: sherpa_onnx_faq
---

### 【sherpa onnx】如何在 .Net 项目中使用 cuda

> 你得有 nvidia GPU 并且 cuda 版本是 11.8
  1. 正常在.net项目中通过 nuget 的方式引入 sherpa-onnx
  2. 正常编译 .net 项目，然后找到对应的 build 目录，去 build 目录里，找到 sherpa-onnx 相关的 .so 文件
  3. 去https://github.com/k2-fsa/sherpa-onnx/releases/tag/v1.10.30 （v1.10.30是版本号，建议找最新的）下载我们提供的编译好的 gpu 版本的 sherpa-onnx 的 .so 文件. 比如，你用 linux x64, 那么，就是  https://github.com/k2-fsa/sherpa-onnx/releases/download/v1.10.30/sherpa-onnx-v1.10.30-linux-x64-gpu.tar.bz2
  4. 用 第3步中得到的 .so 文件，替换掉 第二步中的 .so 文件

