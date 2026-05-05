---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# About me
I am a 4-th year PhD student in the Computer Science department at UC Santa Barbara. I am fortunate to be advised by Professor [Ben Hardekopf](https://sites.cs.ucsb.edu/~benh/) and [Jonathan Balkind](https://jbalkind.github.io/). I obtained my Bachelor degrees in Computer Science from Peking University and was lucky to work with Professor [Yingfei Xiong](https://xiongyingfei.github.io/) as a member of [PKU-PLL](https://pl.cs.pku.edu.cn/en/).

My interests primarily lie in the areas of software engineering and programming languages. 
At present, I am focused on utilizing these techniques to solve problems related to hardware design.

<!-- My name is pronounced as [jin tow sshyah]. -->

# Education
<div class="education-list">
  <div class="education-item">
    <img class="education-logo" src="/images/Ucsbseal.jpg" alt="UC Santa Barbara logo">
    <div class="education-copy">
      <div class="education-header">
        <div class="education-degree">Ph.D., Computer Science</div>
        <div class="education-year">2022-present</div>
      </div>
      <div class="education-school">University of California, Santa Barbara</div>
      <div class="education-advisor">Advisors: <a href="https://sites.cs.ucsb.edu/~benh/">Ben Hardekopf</a> and <a href="https://jbalkind.github.io/">Jonathan Balkind</a></div>
    </div>
  </div>

  <div class="education-item">
    <img class="education-logo" src="/images/pku.png" alt="Peking University logo">
    <div class="education-copy">
      <div class="education-header">
        <div class="education-degree">B.S., Computer Science</div>
        <div class="education-year">2018-2022</div>
      </div>
      <div class="education-school">Peking University</div>
      <div class="education-advisor">Advisor: <a href="https://xiongyingfei.github.io/">Yingfei Xiong</a></div>
    </div>
  </div>
</div>

# Research
**Fungible Memories for Automated Technology Mapping and Re-targeting** <br>
Zachary D. Sisco, Sijie Kong, Daniel Ruelas-Petrisko, **Jingtao Xia**, Julian Springer, Varun Rao, Spencer Wang, Gus Henry Smith, Ben Hardekopf, Jonathan Balkind <br>
*(To Appear) <abbr title="ACM SIGPLAN Conference on Programming Language Design and Implementation">PLDI</abbr> ’26* 

**Improving Equality Saturation for EDA via Semantic E-Graphs** <br>
Sijie Kong\*, **Jingtao Xia**\*, Daniel Ruelas-Petrisko, Zachary D. Sisco, Jonathan Balkind, Gus Henry Smith <br>
*(To Appear) <abbr title="ACM SIGPLAN Conference on Programming Language Design and Implementation">PLDI</abbr> ’26* <br>
\* Equal contribution

**Implementing Cache Coherence with Coroutines: A Case Study** <br>
Andrew David Alex, **Jingtao Xia**, Gus Henry Smith, Rachit Nigam, Jonathan Balkind, Gilbert Bernstein <br>
*<abbr title="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</abbr> ’26* <a href="https://capra.cs.cornell.edu/latte26/paper/latte26-final12.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
Hardware description languages must offer more productive abstractions without sacrificing low-level control. Coroutines are an expressive control construct that naturally describe the progression of a protocol as a sequence of steps separated by yield statements. In this report, we describe our experience modeling a hardware description language with coroutines to implement the MSI cache coherence protocol.
</details>

**Unifying HLS and RTL with Timeline Types** <br>
**Jingtao Xia**, Ayana Alemayehu, Sijie Kong, Ben Hardekopf, Rachit Nigam, Jonathan Balkind <br>
*<abbr title="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</abbr> ’26* <a href="https://capra.cs.cornell.edu/latte26/paper/latte26-final17.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
Hardware design today is divided between two paradigms: RTL offers precise control over timing and resources but demands substantial manual effort, while HLS provides automation at the cost of predictability and fine-grained control. We argue that this dichotomy is unnecessary. This paper proposes a unifying design approach for latency-sensitive and latency-abstract hardware based on timeline types. By extending Filament’s timeline type system with scheduler-determined parameters, denoted by question marks, designers can selectively leave binding and scheduling decisions partially open to automation while retaining explicit control where needed. This enables a continuous spectrum between fully manual RTL design and fully automated HLS design within a single language framework, making it possible to combine fine-grained control with automation.
</details>

**Refinement Types for Visualization** <br>
**Jingtao Xia**, Junrui Liu, Nicholas Brown, Yanju Chen, Yu Feng <br>
*<abbr title="IEEE/ACM International Conference on Automated Software Engineering">ASE</abbr> ’24* <a href="https://dl.acm.org/doi/10.1145/3691620.3695550" title="Paper"><i class="fas fa-file-pdf"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
This paper introduces a visualization-synthesis approach based on refinement types. Users can supplement examples with logical annotations that constrain visualization values or relationships between visual components, and the Calico system uses lightweight bidirectional type checking to efficiently synthesize data transformations and visualizations.
</details>

**There and Back Again: A Netlist's Tale with Much Egraphin'** <br>
Gus Henry Smith, Zachary D Sisco, Thanawat Techaumnuaiwit, **Jingtao Xia**, Vishal Canumalla, Andrew Cheung, Zachary Tatlock, Chandrakana Nandi, Jonathan Balkind 
<br>
*<abbr title="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</abbr> ’24* <a href="https://capra.cs.cornell.edu/latte24/paper/8.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
EDA toolchains are notoriously unpredictable, incomplete, and error-prone; the generally-accepted remedy has been to re-imagine EDA tasks as compilation problems. However, any compiler framework we apply must be prepared to handle the wide range of EDA tasks, including not only compilation tasks like technology mapping and optimization (the "there" in our title), but also decompilation tasks like loop rerolling (the "back again"). In this paper, we advocate for equality saturation -- a term rewriting framework -- as the framework of choice when building hardware toolchains. Through a series of case studies, we show how the needs of EDA tasks line up conspicuously well with the features equality saturation provides.
</details>


**ALGO: Synthesizing Algorithmic Programs with Generated Oracle Verifiers** <br>
Kexun Zhang, Danqing Wang, **Jingtao Xia**, William Yang Wang, Lei Li
 <br>
*<abbr title="Conference on Neural Information Processing Systems">NeurIPS</abbr> 2023* <a href="https://arxiv.org/pdf/2305.14591.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a> <a href="https://github.com/zkx06111/ALGO" title="Source code"><i class="fab fa-github"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
ALGO improves algorithmic code generation by using LLM-generated oracle programs to guide search and verify candidate solutions. The framework is model-agnostic and improves one-submission pass rates on competitive-programming benchmarks by combining generation with automatically produced correctness checks.
</details>


**Generalizable Synthesis Through Unification.** <br>
Ruyi Ji, **Jingtao Xia**, Yingfei Xiong, Zhenjiang Hu. <br>
*<abbr title="ACM SIGPLAN International Conference on Object-Oriented Programming, Systems, Languages, and Applications">OOPSLA</abbr> 2021* <a href="http://jingtaox.github.io/files/OOPSLA21.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a> <a href="https://github.com/jiry17/PolyGen" title="Source code"><i class="fab fa-github"></i></a>
<details class="abstract-toggle">
<summary>Abstract</summary>
The generalizability of PBE solvers is the key to the empirical synthesis performance. Despite the importance of generalizability, related studies on PBE solvers are still limited. In theory, few existing solvers provide theoretical guarantees on generalizability, and in practice, there is a lack of PBE solvers with satisfactory generalizability on important domains such as conditional linear integer arithmetic (CLIA). In this paper, we adopt a concept from the computational learning theory, Occam learning, and perform a comprehensive study on the framework of synthesis through unification (STUN), a state-of-the-art framework for synthesizing programs with nested if-then-else operators. We prove that Eusolver, a state-of-the-art STUN solver, does not satisfy the condition of Occam learning, and then we design a novel STUN solver, PolyGen, of which the generalizability is theoretically guaranteed by Occam learning. We evaluate PolyGen on the domains of CLIA and demonstrate that PolyGen significantly outperforms two state-of-the-art PBE solvers on CLIA, Eusolver and Euphony, on both generalizability and efficiency.
</details>

# Teaching
* CS32: Object-Oriented Design (Fall'24, Winter'26, Spring'26)
* CS138: Automata and Formal Languages (Spring'24, [Fall'25](https://sites.cs.ucsb.edu/~bultan/courses/138/))
* CS9: Intermediate Python ([Fall'23](https://ucsb-cs9.github.io/f23/), [Winter'24](https://ucsb-cs9.github.io/w24/))
* CS160: Translation of Computer Programs ([Spring'23](https://github.com/fredfeng/CS160/))
* CS162:  Programming Languages ([Winter'23](https://github.com/fredfeng/CS162/tree/winter-2022))


# Service
* [PLDI'24](https://pldi24.sigplan.org/track/pldi-2024-pldi-research-artifacts) AEC 
