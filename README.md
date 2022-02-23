Quantumult X入门入门教程<img width="228" alt="0e9480be9870bf8fde60a6d30719ad96" src="https://user-images.githubusercontent.com/96102326/155284616-da7641d5-95a1-4005-bb6f-b8fc10eebf76.png">

电报交流群：https://t.me/xgfxl
一、Quantumult X简介与下载
Quantumult X 简称“X”，是Ray功能强大的网络，工具主要介绍它的代理功能。
Quantumult X目前支持的协议：SS/SSR、V2、Trojan、HTTP(S
) APP，7.99美元，需要美区等AppleID登录用Apple Store下载。

注册美国AppleID教程：https://youtu.be/KOU-PWHMb8o


二、Quantumult X添加节点，订阅链接
1、通过机场订阅链接导入
Quantumult X SS/SSR订阅链接、支持Quantumult X格式的V2Ray和Trojan订阅链接。
机场网站有 Quantumult X 订阅订阅链接的，直接到 X 圈的复制引用（链接）里粘贴，或者点击导入到 Quantum X 。
机场网站没有Quantumult X的订阅链接，SS/SSR订阅链接可以使用，是V2Ray和Trojan订阅链接不能直接导入Quantumult X，如果直接导入Quantumult X，
需要添加一个资源解析器，使用资源解析器后，可以将Quantumult X不识别的节点或链接的导入。
✈️如何添加资源解析器？
打开Quantumult X配置文件，找到[general]位置，添加以下代码：resource_parser_url=https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/resource-parser.js



策略组
1、策略组是什么？
策略组可以实现自动切换节点、偏差筛选、是否走代理等。
策略组需要配合分流规则使用。
可包含多个节点和策略组。
2、Quantumult X自带3种策略。
PROXY（代理）
DIRECT（直连）
REJECT（拒绝）
3、Quantumult X策略组类型
静态静态策略-手动选择节点
可用健康检查-自动选择节点，从第一个节点开始检查是否可用，直到选择可用节点。
轮询平均平均轮询调度，轮流调用使用，IP可能会一直变化。
目标哈希
url-latency-benchmark 自动测速-自动选择延迟低的节点
4、添加策略组（重点）
打开Quantumult X配置文件，找到[policy]位置
策略默认

static=default, proxy, direct, reject



筛选节点的策略组



