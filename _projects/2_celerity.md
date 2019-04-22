---
layout: page
title: Celerity
description: Open-Source RISC-V Tiered Accelerator Fabric SoC.</br> I was one of the most contributors on Celerity projects when I worked in Michael Taylor's group at University of California, San Diego, from 2016 -- 2017. I was in charge of the manycore array, SoC assembling and software stack. 
img: /assets/img/Celerity_logo.svg
---

[Celerity](http://opencelerity.org) is an accelerator-centric system-on-chip (SoC) which uses a tiered accelerator
fabric to improve energy efficiency in the context of high-performance embedded systems.

The SoC is a 5x5 mm2 385 M-transistor chip in TSMC 16 nm designed and
implemented by a modest team of over 20 students and faculty from the University
of Michigan, Cornell University, and the [Bespoke Silicon Group](http://darksilicon.net/group_news)
(now at U. Washington) as part of the **DARPA** Circuit Realization At Faster Timescales (CRAFT) program.

Celerity currently holds the world record for RISC-V performance; 500B RISC-V instructions per second,
beating prior records by 100X.

## SoC Structure
<!-- Description for  different tiers -->
<div align="center"> 

<!-- Description for general  tiers -->
<div style="width:210px; position:relative; display:inline-block; margin-left:3px; float:left">
<img src="{{ site.baseurl }}/assets/img/General-tier.png">
<p align="left"> <strong> General Purpose Tier </strong></p>
<p align="left">A few fully featured RISC-V processors 
capable of running general-purpose software including an operating system.
Modified version of Berkeley Rocket core. </p>
</div>

<!-- Description for Massive tiers -->
<div style="width:210px; position:relative; display:inline-block; margin-left:3px; float:left" >
<img src="{{ site.baseurl }}/assets/img/Massive-tier.png">
<p align="left"> <strong> Massive Parallel Tier </strong> </p>
<p align="left">A manycore comprising hundreds of lightweight RISC-V processors, 
a distributed shared memory system, and a mesh-based interconnect. 
</p>
</div>

<!-- Description for Specialization tiers -->
<div style="width:210px; position:relative; display:inline-block; margin-left:3px; float:left">
<img src="{{ site.baseurl }}/assets/img/Specialization-tier.png">
<p align="left"> <strong> Specialization Tier </strong> </p>
<p align="left"> Application-specific accelerators (possibly 
generated using high-level synthesis). 
</p>
</div>

</div>
<div style="clear:left"> </div>

## Related Links 

* [Official Open Celerity website](opencelerity.org)
* [Celerity Quick Start](https://docs.google.com/document/d/1Sg6TLo4kOI072pgjI43fMVsh7a3-P9shqQdkxhORrCk/view)
* [Source code on Github](https://github.com/bespoke-silicon-group/bsg_manycore)


## Publication

Please cite following paper if you find our research helpful:

```text
@article{davidson2018celerity,
 title={The Celerity open-source 511-core RISC-V tiered accelerator fabric: Fast architectures and design methodologies for fast chips},
 author={Davidson, Scott and Xie, Shaolin and Torng, Christopher and Al-Hawai, Khalid and Rovinski, Austin and Ajayi, Tutu and Vega, Luis and Zhao, Chun and Zhao, Ritchie and Dai, Steve and others},
 journal={IEEE Micro},
 volume={38},
 number={2},
 pages={30--41},
 year={2018},
 publisher={IEEE}
 }
```

{% bibliography -f papers -q @*[title=The Celerity open-source 511-core RISC-V tiered accelerator fabric: Fast architectures and design methodologies for fast chips]* %}
{% bibliography -f papers -q @*[title=Celerity: An open source RISC-V tiered accelerator fabric]* %}
{% bibliography -f papers -q @*[title=The BaseJump Manycore Accelerator Network]* %}
{% bibliography -f papers -q @*[title=Experiences Using the RISC-V Ecosystem to Design an Accelerator-Centric SoC in TSMC 16nm]* %}
