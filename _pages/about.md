---
permalink: /
title: ""
excerpt: ""
author_profile: false
redirect_from: 
  - /about/
  - /about.html
---

<div class="home-intro">
  <figure class="home-intro__figure">
    <img id="home-profile-media" src="/images/profile.png" alt="Jingtao Xia">
  </figure>

  <div class="home-intro__identity">
    <h1>Jingtao Xia <span>夏景涛</span></h1>
    <p class="home-intro__role">Ph.D. Student</p>
    <p class="home-intro__affiliation">
      <a href="https://www.cs.ucsb.edu/">Department of Computer Science</a><br>
      <a href="https://www.ucsb.edu/">University of California, Santa Barbara</a>
    </p>

    <dl class="home-intro__details">
      <div>
        <dt><i class="fas fa-map-marker-alt" aria-hidden="true"></i> Location:</dt>
        <dd>Santa Barbara, CA</dd>
      </div>
      <div>
        <dt><i class="fas fa-envelope" aria-hidden="true"></i> Email:</dt>
        <dd>jingtaoxia@ucsb.edu</dd>
      </div>
    </dl>

    <div class="home-intro__links">
      <a href="https://github.com/JingtaoX"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a>
      <a href="https://www.linkedin.com/in/jingtao-xia"><i class="fab fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
      <a href="https://scholar.google.com/citations?user=ZhTN_5cAAAAJ&hl=en"><i class="fas fa-graduation-cap" aria-hidden="true"></i> Google Scholar</a>
      <a href="https://orcid.org/0009-0007-3509-4018"><i class="ai ai-orcid" aria-hidden="true"></i> ORCID</a>
    </div>
  </div>

  <div class="home-intro__bio">
    <p>I am a 4-th year PhD student in the Computer Science department at UC Santa Barbara. I am fortunate to be advised by Professor <a href="https://sites.cs.ucsb.edu/~benh/">Ben Hardekopf</a> and <a href="https://jbalkind.github.io/">Jonathan Balkind</a>. I obtained my Bachelor degrees in Computer Science from Peking University and was lucky to work with Professor <a href="https://xiongyingfei.github.io/">Yingfei Xiong</a> as a member of <a href="https://pl.cs.pku.edu.cn/en/">PKU-PLL</a>.</p>

    <p>My interests primarily lie in the areas of software engineering and programming languages. At present, I am focused on utilizing these techniques to solve problems related to hardware design.</p>
  </div>
</div>

<script>
  (function () {
    var media = document.getElementById("home-profile-media");
    if (!media) {
      return;
    }

    var profileMedia = [
      {% for file in site.static_files %}
        {% assign ext = file.extname | downcase %}
        {% if file.path contains '/images/profiles/' %}
          {% if ext == '.jpg' or ext == '.jpeg' or ext == '.png' or ext == '.gif' or ext == '.webp' or ext == '.mp4' or ext == '.webm' %}
            { src: "{{ file.path | prepend: base_path }}", ext: "{{ ext }}" },
          {% endif %}
        {% endif %}
      {% endfor %}
    ];

    if (profileMedia.length === 0) {
      return;
    }

    var choice = profileMedia[Math.floor(Math.random() * profileMedia.length)];
    if (choice.ext === ".mp4" || choice.ext === ".webm") {
      var video = document.createElement("video");
      video.id = media.id;
      video.className = media.className;
      video.autoplay = true;
      video.muted = true;
      video.loop = true;
      video.playsInline = true;
      video.setAttribute("aria-label", media.alt);
      video.src = choice.src;
      media.replaceWith(video);
    } else {
      media.src = choice.src;
    }
  }());
</script>

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
<div class="publication-item">
  <div class="publication-title">Fungible Memories for Automated Technology Mapping and Re-targeting</div>
  <div class="publication-authors">Zachary D. Sisco, Sijie Kong, Daniel Ruelas-Petrisko, <strong>Jingtao Xia</strong>, Julian Springer, Varun Rao, Spencer Wang, Gus Henry Smith, Ben Hardekopf, Jonathan Balkind</div>
  <div class="publication-meta">
    <span class="publication-meta-item">(To Appear) <span class="venue-tooltip" data-tooltip="ACM SIGPLAN Conference on Programming Language Design and Implementation">PLDI</span> ’26</span>
  </div>
</div>

<div class="publication-item">
  <div class="publication-title">Improving Equality Saturation for EDA via Semantic E-Graphs</div>
  <div class="publication-authors">Sijie Kong*, <strong>Jingtao Xia</strong>*, Daniel Ruelas-Petrisko, Zachary D. Sisco, Jonathan Balkind, Gus Henry Smith</div>
  <div class="publication-meta">
    <span class="publication-meta-item">(To Appear) <span class="venue-tooltip" data-tooltip="ACM SIGPLAN Conference on Programming Language Design and Implementation">PLDI</span> ’26</span>
  </div>
  <div class="publication-note">* Equal contribution</div>
</div>

<div class="publication-item">
  <div class="publication-title">Implementing Cache Coherence with Coroutines: A Case Study</div>
  <div class="publication-authors">Andrew David Alex, <strong>Jingtao Xia</strong>, Gus Henry Smith, Rachit Nigam, Jonathan Balkind, Gilbert Bernstein</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</span> ’26</span>
    <span class="publication-meta-item"><a href="https://capra.cs.cornell.edu/latte26/paper/latte26-final12.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    Hardware description languages must offer more productive abstractions without sacrificing low-level control. Coroutines are an expressive control construct that naturally describe the progression of a protocol as a sequence of steps separated by yield statements. In this report, we describe our experience modeling a hardware description language with coroutines to implement the MSI cache coherence protocol.
  </details>
</div>

<div class="publication-item">
  <div class="publication-title">Unifying HLS and RTL with Timeline Types</div>
  <div class="publication-authors"><strong>Jingtao Xia</strong>, Ayana Alemayehu, Sijie Kong, Ben Hardekopf, Rachit Nigam, Jonathan Balkind</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</span> ’26</span>
    <span class="publication-meta-item"><a href="https://capra.cs.cornell.edu/latte26/paper/latte26-final17.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    Hardware design today is divided between two paradigms: RTL offers precise control over timing and resources but demands substantial manual effort, while HLS provides automation at the cost of predictability and fine-grained control. We argue that this dichotomy is unnecessary. This paper proposes a unifying design approach for latency-sensitive and latency-abstract hardware based on timeline types. By extending Filament’s timeline type system with scheduler-determined parameters, denoted by question marks, designers can selectively leave binding and scheduling decisions partially open to automation while retaining explicit control where needed. This enables a continuous spectrum between fully manual RTL design and fully automated HLS design within a single language framework, making it possible to combine fine-grained control with automation.
  </details>
</div>

<div class="publication-item">
  <div class="publication-title">Refinement Types for Visualization</div>
  <div class="publication-authors"><strong>Jingtao Xia</strong>, Junrui Liu, Nicholas Brown, Yanju Chen, Yu Feng</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="IEEE/ACM International Conference on Automated Software Engineering">ASE</span> ’24</span>
    <span class="publication-meta-item"><a href="https://dl.acm.org/doi/10.1145/3691620.3695550" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    This paper introduces a visualization-synthesis approach based on refinement types. Users can supplement examples with logical annotations that constrain visualization values or relationships between visual components, and the Calico system uses lightweight bidirectional type checking to efficiently synthesize data transformations and visualizations.
  </details>
</div>

<div class="publication-item">
  <div class="publication-title">There and Back Again: A Netlist's Tale with Much Egraphin'</div>
  <div class="publication-authors">Gus Henry Smith, Zachary D Sisco, Thanawat Techaumnuaiwit, <strong>Jingtao Xia</strong>, Vishal Canumalla, Andrew Cheung, Zachary Tatlock, Chandrakana Nandi, Jonathan Balkind</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="Workshop on Languages, Tools, and Techniques for Accelerator Design">LATTE</span> ’24</span>
    <span class="publication-meta-item"><a href="https://capra.cs.cornell.edu/latte24/paper/8.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    EDA toolchains are notoriously unpredictable, incomplete, and error-prone; the generally-accepted remedy has been to re-imagine EDA tasks as compilation problems. However, any compiler framework we apply must be prepared to handle the wide range of EDA tasks, including not only compilation tasks like technology mapping and optimization (the "there" in our title), but also decompilation tasks like loop rerolling (the "back again"). In this paper, we advocate for equality saturation -- a term rewriting framework -- as the framework of choice when building hardware toolchains. Through a series of case studies, we show how the needs of EDA tasks line up conspicuously well with the features equality saturation provides.
  </details>
</div>

<div class="publication-item">
  <div class="publication-title">ALGO: Synthesizing Algorithmic Programs with Generated Oracle Verifiers</div>
  <div class="publication-authors">Kexun Zhang, Danqing Wang, <strong>Jingtao Xia</strong>, William Yang Wang, Lei Li</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="Conference on Neural Information Processing Systems">NeurIPS</span> 2023</span>
    <span class="publication-meta-item"><a href="https://arxiv.org/pdf/2305.14591.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
    <span class="publication-meta-item"><a href="https://github.com/zkx06111/ALGO" title="Source code"><i class="fab fa-github"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    ALGO improves algorithmic code generation by using LLM-generated oracle programs to guide search and verify candidate solutions. The framework is model-agnostic and improves one-submission pass rates on competitive-programming benchmarks by combining generation with automatically produced correctness checks.
  </details>
</div>

<div class="publication-item">
  <div class="publication-title">Generalizable Synthesis Through Unification.</div>
  <div class="publication-authors">Ruyi Ji, <strong>Jingtao Xia</strong>, Yingfei Xiong, Zhenjiang Hu.</div>
  <div class="publication-meta">
    <span class="publication-meta-item"><span class="venue-tooltip" data-tooltip="ACM SIGPLAN International Conference on Object-Oriented Programming, Systems, Languages, and Applications">OOPSLA</span> 2021</span>
    <span class="publication-meta-item"><a href="http://jingtaox.github.io/files/OOPSLA21.pdf" title="Paper"><i class="fas fa-file-pdf"></i></a></span>
    <span class="publication-meta-item"><a href="https://github.com/jiry17/PolyGen" title="Source code"><i class="fab fa-github"></i></a></span>
  </div>
  <details class="abstract-toggle">
    <summary>Abstract</summary>
    The generalizability of PBE solvers is the key to the empirical synthesis performance. Despite the importance of generalizability, related studies on PBE solvers are still limited. In theory, few existing solvers provide theoretical guarantees on generalizability, and in practice, there is a lack of PBE solvers with satisfactory generalizability on important domains such as conditional linear integer arithmetic (CLIA). In this paper, we adopt a concept from the computational learning theory, Occam learning, and perform a comprehensive study on the framework of synthesis through unification (STUN), a state-of-the-art framework for synthesizing programs with nested if-then-else operators. We prove that Eusolver, a state-of-the-art STUN solver, does not satisfy the condition of Occam learning, and then we design a novel STUN solver, PolyGen, of which the generalizability is theoretically guaranteed by Occam learning. We evaluate PolyGen on the domains of CLIA and demonstrate that PolyGen significantly outperforms two state-of-the-art PBE solvers on CLIA, Eusolver and Euphony, on both generalizability and efficiency.
  </details>
</div>

# Teaching
* CS32: Object-Oriented Design (Fall'24, Winter'26, Spring'26)
* CS138: Automata and Formal Languages (Spring'24, [Fall'25](https://sites.cs.ucsb.edu/~bultan/courses/138/))
* CS9: Intermediate Python ([Fall'23](https://ucsb-cs9.github.io/f23/), [Winter'24](https://ucsb-cs9.github.io/w24/))
* CS160: Translation of Computer Programs ([Spring'23](https://github.com/fredfeng/CS160/))
* CS162:  Programming Languages ([Winter'23](https://github.com/fredfeng/CS162/tree/winter-2022))


# Service
* [PLDI'24](https://pldi24.sigplan.org/track/pldi-2024-pldi-research-artifacts) AEC 
