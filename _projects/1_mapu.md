---
layout: page
title: MaPU
description: A Mathematical Computing Architecture. </br> MaPU was based on my PhD dissertation which assembles the data path based on program flow. From 2009 - 2016 when I worked as a research scientist at Chinese Academy of Science, I lead the team (initially only PhD students) to implement the architecture spanning from programming model, software and hardware.
img: /assets/img/MaPU_logo.svg
---

MaPU (**Ma**thematical **P**rocessing **U**nit) is a novel architecture targeting data-intensive computing with great power efficiency and sustained computation throughput.  

To achieve this goal, MaPU uses mathematical formulates style program model, directly mapped data path on CGRA fabric and groundbreaking memory system that supports simultaneous row-major and column major matrix with the same layout. 
<div class="img_row">
    <img class="col three left" src="{{ site.baseurl }}/assets/img/MaPU_APE.svg" alt="" title="MaPU Architecture"/>
</div>

<div class="col three caption">
    The Function Unit (FU) are connected via a cross bar to form a CGRA farbic
</div>

## Toolchains

MaPU toolchain includes assembler/disassembler, compiler, simulator etc., for both scalar pipeline and micro-code pipeline.
Complete source code can be found at [https://github.com/mapu/toolchains.git](https://github.com/mapu/toolchains.git).

|Tool name                                   | Based Open Source Framework   |
|--------------------------------------------|-------------------------------|
|Compiler for State Machine based language   | Ragel &Bison & LLVM           |
|C compiler for Scalar Pipeline              | Clang & LLVM                  |
|Assembler /Disassembler                     | Ragel & Bison & LLVM          |
|Linker                                      | Binutils Gold                 |
|Debugger for Scalar Pipeline                | GDB                           |
|Simulator ( Scalar & Microcode )            | Gem5                          |
|Emulator                                    | OpenOCD                       |
|--------------------------------------------|-------------------------------|

## Prototype Chip

<div class="img_row">
    <img class="one three left" src="{{ site.baseurl }}/assets/img/MaPU_layout.svg" alt="" title="MaPU Layout"/>
    <img class="two three left" src="{{ site.baseurl }}/assets/img/MaPU_Chip.jpeg" alt="" title="MaPU Chip"/>
</div>
<div class="col three caption">
    Left: Layout of a MaPU Core. Right: Packaged 40nm chip.
</div>

## Chip Performance
<div class="img_row">
    <img class="col three left" src="{{ site.baseurl }}/assets/img/MaPU_Performance.svg" alt="" title="MaPU Performance"/>
</div>
<div class="col three caption">
    Performance chart. 
</div>

## Publication

Please cite our [HPCA'16](https://ieeexplore.ieee.org/abstract/document/7446086) paper if you are inspired our work:
```text
@inproceedings{wang2016mapu,
  title={MaPU: A novel mathematical computing architecture},
  author={Wang, Donglin and Xie, Shaolin and others},
  booktitle={2016 IEEE International Symposium on High Performance Computer Architecture (HPCA)},
  pages={457--468},
  year={2016},
  organization={IEEE}
}
```
### Patents

{% bibliography -f papers -q @*[publisher=Google Patents]* %}
