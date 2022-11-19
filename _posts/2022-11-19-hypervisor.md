---
layout: post
title: 하이퍼바이저 (Hypervisor)
categories: 컴퓨터기초
tags: [ncloud, basic]
---

Hypervisor는 Host OS에서 다수의 Guest OS를 동시에 실행하기 위한 논리적 플랫폼이다.<br>
VM (가상머신)을 생성하고 구동하는 역할을 한다.

![하이퍼바이저](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Hyperviseur.svg/471px-Hyperviseur.svg.png)<br>

Hypervisor에는 type1과 type2가 있는데

type1은 Host OS없이 H/W에서 직접 실행 되며 그 위에서 Guest OS가 실행된다.<br>
type1 S/W로는
Xen, ESX server, TRANGO, Hyper-V 등이 있다.

type2는 H/W에 Host OS가 있고 그 위의 Hypervisor가 Guest OS를 실행한다.<br>
type2 S/W로는
Virtual box, VMware, Parallels 등이 있다. 

그러나 Hypervisor만으로는 VM 생성이 번거롭다.
VM을 생성하고, VM에 OS를 설치하고, 일일이 설정해줘야 하기 때문이다.

그렇게 해서 만들어진 것이 Vagrant이다.
Vagrant는 VM 생성 과정의 반복 작업을 자동화해주는 VM 관리 소프트웨어다.
Vagrant가 있으면 명령어를 통해 손쉽게 VM 생성 및 Guest OS 설치를 할 수 있게 된다.