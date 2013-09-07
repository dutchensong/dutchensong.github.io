---
layout: post
title: "在科技公司工作，你要有工程师思想"
description: "工程师思想就是用自动化或者流程化手段，让复杂的工作变得有序，准确得进行。"
category: 
tags: []
---
{% include JB/setup %}


从事Product Manager和Account Manager的工作快一年了。在这一年中，经历了AppFlood这个产品从无到有，从婴儿期到与国际接轨。每一个阶段都是新的探索。在这个产品上，我没有从事任何开发工作，但在工作方式上，我保持了某种程度的工程师思想，并且我认为这对我，和整个工作的进展都是非常有帮助。

什么是工程师思想呢？那就是通过技术，让机器去代替人做一些重复性高，或是复杂的事情。但这不仅仅限于工程师，所以我把这个思想扩展成：通过技术，或是流程化手段，将一些重复性，或者是复杂的工作变成一段程序，或是像一段程序一样执行。

越是大的公司，流程化，自动化的作用更是重要。但是大部分的创业公司基本处于这样一种状态：跑步前进，工程师档期排满，全部资源都放在主线产品的开发上。在这时候极易产生的情况就是产品，运营，支持人员对于数据，配置等方面的诉求无法得到足够的工程师支持。于是出现了这样的一些情况：

产品，运营，支持人员跑去数据库查数据，甚至敲python代码查数据(当然是工程师给的方法)；
集成，测试，配置手动化成分很高，没有纠错提示(尤其是像我们这种面向developer的产品，技术集成很多)；
对于一些开发者的特殊需求，需要复杂的手动操作完成
这些都是我曾经面对过，或是现在还在面对的事情。理想情况下就是能有工程师资源来把这一系列事情都做成可视化操作界面。但是事情不是总会那么理想，尤其是在跑步前进的创业公司。用工程师思想来解决这些问题，会对提高工作效率有大大的帮助。这里解决问题的核心就是：自动化和流程化。

案例一：从去年11月份开始，到今年3，4月份都是我们产品开始进行开发者server端集成的探索和成长期。在这期间我们完成了所有世界上流行的集成方式的支持与对接。我当时在美国办公室，工作是跟开发者确定技术方案，明确需求看是否需要开发支持，测试和配置上线。从测试到配置上线，我会在手机，电脑，数据库，服务器python环境，log服务器之间各种穿梭。中间包括各种肉体查错，肉体测试等等。如果测试或是配置失误，都可能导致一些问题。

回国之后，我开始利用工作之余写文档。目的是把各种复杂的集成方式归类，每个类别再明确流程和方法。几十页的文档不多，但是这些文档定义了所有的集成方式，每种集成方式的原理以及配置流程。这为我，也为所有做这些事的同事提供了方便，还为新从事这个工作的同事提供了参考。之后，排到了工程师资源，根据我们的需求上线了管理后台，可能管理后台相关功能开发只需要工程师1-2天时间，但是效率的提高是显著的：原来经过七八个流程，耗费可能长达几个小时，并且需要等每天服务器重启才能生效的配置，现在变成了几个click，一个小时就生效并达到上线状态。

这体现了流程化和自动化的强大效果。作为非工程师，时刻总结流程，推进自动化进程是很重要的。

案例二：有个开发者提了一种数据统计需求，要求我们每天给他们发一个数据报表。但是我们系统中没有做相应的统计。

刚开始的解决方案是这样的，拿到一个最原始的数据表，放在excel里面，然后用各种excel手动操作来完成最后满足需求的汇总。过程耗时几个小时。结果给了对方之后，发现数据不对。后来经历了多次重新汇总，耗费了前后有一两天时间之后，终于汇总出了比较正确的数据。这种汇总方式操作熟练之后，可以缩短到半个小时之内出数据。

因为觉得这样太麻烦，所以ask engineer for help!找了我们后端工程师帮忙汇总一份算是半成品数据。这份数据拿过来再操作，在excel里面就简单多了，但我觉得这还是太手动，不值得为一个这种特殊需求每天花那些时间去手动做表。

于是乎，自己动手。因为半成品数据已经有了，我开始重拾代码，工作之余用python写了个脚本来处理那个半成品数据，直接一步到位处理成满足需求的成品。每天跑数据，只需要运行一下那个python文件，耗时几乎是0

数据已经跑了两三个月。如果按照每天节省10分钟，已经节省出来八个多小时。也就是一天时间。如果没有写自动化脚本，那我过去的两三个月花费了1整天来做对自己和自己的产品毫无意义的excel操作。。。

当然作为非技术人员不一定要亲自写代码，但是一定要有意识来避免这些无意义而又完全重复的工作。

我遇到的问题有的已经解决，有的还等待解决，提高工作效率的方式很多，欢迎一起交流。