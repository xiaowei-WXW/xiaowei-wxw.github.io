---
layout: page
---

# About Me

<img src="/images/XIAOWEI WU.png" class="floatpic">

Here is **Xiaowei Wu**.<br>

I am a Ph.D. Candidate in the Department of [Materials Engineering](https://mtm.kuleuven.be/english) at the [Metal Performance Innovation (Elooi) Laboratory](https://www.mtm.kuleuven.be/english/research/elooi/) of the **KU Leuven**. Currently, I build **data-driven approaches and computational models** for dented thin sheet metals, spanning 3D surface metrology (point-cloud segmentation and parametric modelling), mechanical response simulation with **Finite-Element Analysis**, structural integrity assessment, and **Machine Learning** for remaining useful life prediction. Broadly, my interests lie at the intersection of **fatigue and fracture mechanics, impact dent damage, structural integrity, numerical simulation and machine learning**. Prior to joining KU Leuven, I gained valuable research experiences as a Master's student at Harbin Institute of Technology advised by [Prof. Xiaoguo Song](https://scholar.google.com/citations?user=XIiWmtIAAAAJ&hl=zh-CN). My work focused on **ultrasonic-assisted active-metal soldering**, **interfacial characterisation**, and **dissimilar-material processing**. I developed and analyzed advanced heat-treatment processes, conducted extensive microstructural characterisations, and applied these techniques to structural composite materials, resulting in four journal publications and one granted patent.<br>

## Work Experience

<div class="timeline">
  <div class="timeline-progress" id="timeline-progress"></div>

  <div class="timeline-item timeline-item--current">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/kuleuven.svg" alt="KU Leuven">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Ph.D. Candidate <span class="timeline-sep">|</span> <span class="timeline-company">KU Leuven</span></div>
        <span class="timeline-time">Mar. 2023 - Jan. 2027</span>
      </div>
      <div class="timeline-details">
        Developed an inspection-driven framework connecting 3D dent morphology to local mechanical states and fatigue performance through parametric geometry descriptors. Built finite-element models and established machine learning models for residual-stress assessment and remaining-useful-life prediction.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/hit.png" alt="Harbin Institute of Technology">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Master's Researcher <span class="timeline-sep">|</span> <span class="timeline-company">Harbin Institute of Technology</span></div>
        <span class="timeline-time">Sep. 2020 - Sep. 2022</span>
      </div>
      <div class="timeline-details">
        Investigated the bonding mechanism and process-property relationship of ultrasound-induced low-temperature active-metal soldering of quartz glass using Sn-Ti alloy. Characterised interfacial reactions and microstructural evolution.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/tyut.jpg" alt="Taiyuan University of Technology">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Undergraduate Researcher <span class="timeline-sep">|</span> <span class="timeline-company">Taiyuan University of Technology</span></div>
        <span class="timeline-time">Aug. 2018 - Jun. 2020</span>
      </div>
      <div class="timeline-details">
        Fabricated copper-steel composite sheets via friction-stir additive manufacturing and characterised the dissimilar-material interface. Developed a heat-treatment route for NiTi alloy with controllable dual-memory effect and designed a support structure using finite-element analysis.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/henrey.png" alt="HENREY AUTOMOBILE">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Formula Student Intern <span class="timeline-sep">|</span> <span class="timeline-company">HENREY AUTOMOBILE</span></div>
        <span class="timeline-time">Jul. 2018 - Aug. 2018</span>
      </div>
      <div class="timeline-details">
        Served as a Formula Student car-body intern, responsible for schedule coordination, small-assembly design, and technical training.
      </div>
    </div>
  </div>

</div>

<script>
(function() {
  var timelineProgress = document.getElementById('timeline-progress');
  var timeline = document.querySelector('.timeline');
  if (!timelineProgress || !timeline) return;

  var items = timeline.querySelectorAll('.timeline-item');

  // IntersectionObserver for in-view class
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('in-view');
        }
      });
    }, { rootMargin: '0px 0px -15% 0px' });

    items.forEach(function(item, idx) {
      if (idx < 3) {
        // Reveal first 3 immediately on load (still gets the stagger transition)
        item.classList.add('in-view');
      } else {
        observer.observe(item);
      }
    });
  } else {
    items.forEach(function(item) { item.classList.add('in-view'); });
  }

  // Scroll progress bar
  window.addEventListener('scroll', function() {
    var rect = timeline.getBoundingClientRect();
    var totalHeight = timeline.offsetHeight;
    var windowH = window.innerHeight;
    var lineTop = 30;
    var lineBottom = 30;
    var lineHeight = totalHeight - lineTop - lineBottom;

    if (rect.top < windowH && rect.bottom > 0) {
      var scrolled = Math.min(1, Math.max(0, (windowH - rect.top - lineTop) / (totalHeight - lineTop + windowH * 0.4)));
      timelineProgress.style.height = Math.min(scrolled * lineHeight, lineHeight) + 'px';
    }
  }, { passive: true });
})();
</script>

If you are interested in any aspect of me, I am always open to discussions and collaborations. Feel free to reach out to me at - xiaowei.wu@kuleuven.be

**<font color="#990000">Seeking Materials/Mechanical Engineering roles — Fatigue & Fracture Mechanics, 3D Metrology, and Predictive Modeling. Feel free to reach out!</font>**

---

## Publications

<h3 class="section-title">Journal Publications</h3>
<div class="publications-grid">

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper1.jpg" alt="Inspection-driven remaining useful life prediction">
      <a href="https://doi.org/10.1016/j.ijfatigue.2026.109837" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1016/j.ijfatigue.2026.109837" target="_blank" rel="noopener">Inspection-driven remaining useful life prediction of dented thin plates using a stacking ensemble with physics-based validation</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Sanjay Gothivarekar, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">International Journal of Fatigue, 2026</span> <a href="https://doi.org/10.1016/j.ijfatigue.2026.109837" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, first author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper2.jpg" alt="Quantitative stress assessment of dented fuselage panels">
      <a href="https://doi.org/10.1016/j.aei.2026.104656" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1016/j.aei.2026.104656" target="_blank" rel="noopener">Quantitative stress assessment of dented fuselage panels through the integration of FEM, parametric modeling and Gaussian process regression</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Sanjay Gothivarekar, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">Advanced Engineering Informatics, 2026</span> <a href="https://doi.org/10.1016/j.aei.2026.104656" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, first author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper3.jpg" alt="Analysing crack evolution in wind turbine bearings">
      <a href="https://doi.org/10.1016/j.engfailanal.2024.108839" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1016/j.engfailanal.2024.108839" target="_blank" rel="noopener">Analysing crack evolution in wind turbine bearings using an oscillation-unified model</a>
      </div>
      <div class="publication-authors">S. Wang, J. Du, C. Li, S. Jiang, <strong class="author-highlight">Xiaowei Wu</strong>, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">Engineering Failure Analysis, 2024</span> <a href="https://doi.org/10.1016/j.engfailanal.2024.108839" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, co-author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper4.jpg" alt="Bonding mechanisms of SiO2 glass and 1060 Al">
      <a href="https://doi.org/10.12073/j.cw.20230308001" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.12073/j.cw.20230308001" target="_blank" rel="noopener">Bonding mechanisms of SiO2 glass and 1060 Al by ultrasonic assisted active metal soldering process</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, J. Fu, S. Wei, H. Dong, J. Wang, H. Wang, Xiaoguo Song, Z. Li</div>
      <div class="publication-conference"><span class="pub-venue">China Welding, 2023</span> <a href="https://doi.org/10.12073/j.cw.20230308001" target="_blank">[paper]</a></div>
      <div class="publication-details">first author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper5.jpg" alt="Bonding mechanism of ultrasonically soldered silica glasses">
      <a href="https://doi.org/10.1016/j.matlet.2021.131490" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1016/j.matlet.2021.131490" target="_blank" rel="noopener">Bonding mechanism of ultrasonically soldered silica glasses using tin-titanium solder filler</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Z. Li, Xiaoguo Song, H. Dong, X. Yang, Y. Li, S. Wei, J. Fu</div>
      <div class="publication-conference"><span class="pub-venue">Materials Letters, 2022</span> <a href="https://doi.org/10.1016/j.matlet.2021.131490" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, first author</div>
    </div>
  </div>
  
  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper6.jpg" alt="Microstructure and properties of copper-steel bimetallic sheets">
      <a href="https://doi.org/10.1016/j.jmapro.2022.08.022" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://doi.org/10.1016/j.jmapro.2022.08.022" target="_blank" rel="noopener">Microstructure and properties of copper-steel bimetallic sheets prepared by friction stir additive manufacturing</a>
      </div>
      <div class="publication-authors">Y. Guo, <strong class="author-highlight">Xiaowei Wu</strong>, G. Ren, Z. Liu, R. Yuan, X. Yang, Peng Dong</div>
      <div class="publication-conference"><span class="pub-venue">Journal of Manufacturing Processes, 2022</span> <a href="https://doi.org/10.1016/j.jmapro.2022.08.022" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, co-author</div>
    </div>
  </div>

</div>


<br>
<h3 class="section-title">Conference Presentations</h3>
<div class="publications-grid">

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/conf1.jpeg" alt="ECF25 Conference">
    </div>
    <div class="publication-info">
      <div class="publication-title">
        Interpretable physics-guided CNN for remaining useful life prediction of impact-dented fuselage
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Sanjay Gothivarekar, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">25th European Conference on Fracture (ECF25)</span></div>
      <div class="publication-details">Presentation | Athens, Greece, Sep. 2026 | LIRIAS 4443194</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/conf2.jpg" alt="FABER Conference">
    </div>
    <div class="publication-info">
      <div class="publication-title">
        Physics-informed RUL assessment of impacted aluminum panels using stacking ensemble model
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong></div>
      <div class="publication-conference"><span class="pub-venue">FABER Conference 2026</span></div>
      <div class="publication-details">Presentation | Hvar, Croatia, May 2026 | LIRIAS 4425152</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/conf3.jpeg" alt="BDFM-2025">
    </div>
    <div class="publication-info">
      <div class="publication-title">
        Fatigue Life Prediction of Dented Thin Sheet Metals Using Critical Plane-Based Multiaxial Fatigue Model
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Sanjay Gothivarekar, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">4th Benelux Damage and Fracture Mechanics Network Meeting (BDFM)</span></div>
      <div class="publication-details">Presentation | Antwerp, Belgium, Oct. 2025 | LIRIAS 4405745</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/conf4.jpeg" alt="3rd BDFM">
    </div>
    <div class="publication-info">
      <div class="publication-title">
        Fatigue Performance and Remaining Lifetime Prediction of Dented Thin Sheet Metals Using Data Driven Approach
      </div>
      <div class="publication-authors"><strong class="author-highlight">Xiaowei Wu</strong>, Sanjay Gothivarekar, Reza Talemi</div>
      <div class="publication-conference"><span class="pub-venue">3rd Benelux Damage and Fracture Mechanics Network Meeting</span></div>
      <div class="publication-details">Presentation | Antwerp, Belgium, 2023 | LIRIAS 4263292</div>
    </div>
  </div>

</div>

<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -40px 0px' });
    document.querySelectorAll('.publication-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.publication-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();
</script>

---

## Research Interests

<!-- - ML Systems & AI Infrastructure
- Efficient & On-Device Inference (Apple MLX, [SGLang](https://github.com/sgl-project/sglang)<a class="sgl-badge" href="https://github.com/sgl-project/sglang" target="_blank" rel="noopener noreferrer" aria-label="SGLang on GitHub (opens in a new tab)" title="SGLang on GitHub"><img src="/images/sglang-mark.svg" alt="SGLang logo" width="22" height="25" loading="lazy"></a>)
- Agentic AI (multi-agent orchestration & tool use)
- Machine Learning
- Nonparametric Statistics

I currently work at the intersection of **AI infrastructure and applied ML**, building agent runtimes and optimizing LLM inference.

Previously, my research centered on **nonparametric statistics** and **measurement-error modeling**, unobservable-variable estimation under multiplicative distortion frameworks, where I developed calibration methods and simulation studies to improve correlation-coefficient estimation in complex industrial settings, resulting in five SCI publications.
<img src="/images/sunset.jpg"> -->
- Fatigue & Fracture Mechanics
- Computational Mechanics (Finite-Element Analysis, Abaqus)
- Data-Driven Assessment (Machine Learning, Ensemble Learning, Gaussian Process)
- 3D Surface Metrology & Digital Image Correlation (DIC)
- Dissimilar-Material Processing & Interfacial Characterisation

I currently work at the intersection of **structural integrity, computational mechanics, and applied machine learning**. I build data-driven frameworks and finite-element models to assess residual stress and predict the remaining useful life (RUL) of impact-dented thin sheet structures.

Previously, my research centered on **ultrasonic-assisted active-metal soldering** and **dissimilar-material processing**. I investigated interfacial bonding mechanisms, developed advanced heat-treatment routes, and conducted extensive microstructural characterisations (SEM, EBSD, XRD) for structural composite materials, resulting in six journal publications and a granted patent.
<img src="/images/Interest.jpeg">
---

## News and Updates

<div class="news-grid">
  <div class="news-card news-card--milestone news-card--feature">
    <div class="news-meta">
      <span class="news-date">September 2026</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Presenting our research on interpretable physics-guided CNNs for remaining useful life prediction of impact-dented fuselage at the <strong>25th European Conference on Fracture (ECF25)</strong> in Athens, Greece.</p>

    <div class="milestone-gallery">
      <figure class="mtile">
        <img src="/images/milestones/Team.jpeg" alt="Xiaowei Wu presenting at ECF25 in Athens" loading="lazy">
      </figure>

      <!-- ECF25 Conference cover -->
      <a class="mtile mtile--link mtile--contain" href="https://www.ecf25.eu/en" target="_blank" rel="noopener noreferrer" aria-label="ECF25 Official Website (opens in a new tab)">
        <img src="/images/milestones/ecf25-presentation.png" alt="25th European Conference on Fracture" loading="lazy">
        <span class="mtile__ext" aria-hidden="true">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17 17 7"/><path d="M8 7h9v9"/></svg>
        </span>
        <span class="mtile__cap">
          <span class="mtile__cap-title">ECF25 Conference</span>
          <span class="mtile__cap-domain">ecf25.eu</span>
        </span>
      </a>

      <!-- KU Leuven Elooi Lab cover -->
      <a class="mtile mtile--link" href="https://www.ecf25.eu/en/program" target="_blank" rel="noopener noreferrer" aria-label="KU Leuven Elooi Lab (opens in a new tab)">
        <img src="/images/milestones/Presentation.jpg" alt="Metal Performance Innovation Lab at KU Leuven" loading="lazy">
        <span class="mtile__ext" aria-hidden="true">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17 17 7"/><path d="M8 7h9v9"/></svg>
        </span>
        <span class="mtile__cap">
          <span class="mtile__cap-title">Elooi Lab</span>
          <span class="mtile__cap-domain">kuleuven.be</span>
        </span>
      </a>
    </div>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">2026</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p>First-Author Paper: <a href="https://doi.org/10.1016/j.ijfatigue.2026.109837"><strong>Inspection-driven remaining useful life prediction of dented thin plates using a stacking ensemble with physics-based validation</strong></a> published in <a href="https://www.sciencedirect.com/journal/international-journal-of-fatigue">International Journal of Fatigue</a>.</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">2026</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p>First-Author Paper: <a href="https://doi.org/10.1016/j.aei.2026.104656"><strong>Quantitative stress assessment of dented fuselage panels through the integration of FEM, parametric modeling and Gaussian process regression</strong></a> published in <a href="https://www.sciencedirect.com/journal/advanced-engineering-informatics">Advanced Engineering Informatics</a>.</p>
  </div>

  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">March 2023</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Excited to join the <a href="https://www.mtm.kuleuven.be/english/research/elooi"><strong>Metal Performance Innovation (Elooi) Laboratory</strong></a> at <strong>KU Leuven</strong> as a Ph.D. Candidate under the supervision of Prof. Reza Talemi!</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">2022</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p>First-Author Paper: <a href="https://doi.org/10.1016/j.matlet.2021.131490"><strong>Bonding mechanism of ultrasonically soldered silica glasses using tin-titanium solder filler</strong></a> published in <a href="https://www.sciencedirect.com/journal/materials-letters">Materials Letters</a>.</p>
  </div>
  
  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">May 2020</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Patent Granted! Our invention on <a href="#">Fe-Cu-HEA high-strength, high-toughness biomimetic composite material</a> is officially granted (CN109016728B).</p>
  </div>
</div>



<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -60px 0px' });
    document.querySelectorAll('.news-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.news-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();


