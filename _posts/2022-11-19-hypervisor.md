---
layout: post
title: 하이퍼바이저 (Hypervisor)
categories: 컴퓨터기초
tags: [ncloud]
---

Hypervisor는 Host OS에서 다수의 Guest OS를 동시에 실행하기 위한 논리적 플랫폼이다.
VM (가상머신)을 생성하고 구동하는 역할을 한다.

![하이퍼바이저](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Hyperviseur.svg/471px-Hyperviseur.svg.png)<br>

Hypervisor에는 type1과 type2가 있는데

type1은 Host OS없이 H/W에서 직접 실행 되며 그 위에서 Guest OS가 실행된다.
type1 S/W로는
Xen, ESX server, TRANGO, Hyper-V 등이 있다.

type2는 H/W에 Host OS가 있고 그 위의 Hypervisor가 Guest OS를 실행한다.
type2 S/W로는
Virtual box, VMware, Parallels 등이 있다. 