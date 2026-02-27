---
layout: about
title: Piero Romare
permalink: /

profile:
  align: right
  image: false
  image_circular: false # crops the image to make it circular
  address: false

news: false  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page


---
---

Piero Romare is a PhD Student in Usable Privacy and Security at [Chalmers University of Technology](https://www.chalmers.se), Gothenburg (Sweden), supervised by [prof. Simone Fischer-Hübner](https://scholar.google.com/citations?user=Bb3cL_EAAAAJ&hl=en), co-supervised by [prof. Morten Fjeld](https://scholar.google.com/citations?hl=en&user=ZQhqxscAAAAJ) and [Dr. Farzaneh Karegar](https://scholar.google.com/citations?hl=en&user=p1M0AToAAAAJ) funded by [WASP Wallenberg AI, Autonomous Systems and Software Program](https://wasp-sweden.org). 

He obtained a bachelor degree in Cognitive Psychology at the Department of General Psychology and a master degree in Data Science at the Department of Mathematics from the [University of Padua](https://www.unipd.it/en/) (Italy). 

He has collaborated with [SPRITZ Security and Privacy Research Group](https://spritz.math.unipd.it) led by [prof. Mauro Conti](https://scholar.google.com/citations?user=0BcsOY8AAAAJ&hl=en&oi=ao) and with [Ubiquitous Interaction Research Group](https://www.helsinki.fi/en/researchgroups/ubiquitous-interaction) at the [University of Helsinki](https://www.helsinki.fi/en) (Finland) led by [prof. Giulio Jacucci](https://scholar.google.com/citations?hl=en&user=cmpzu9sAAAAJ).

---
<a href="/assets/pdf/CV.pdf" target="_blank" rel="noopener noreferrer" class="float-right" style="margin-right: 20px;"><i class="fas fa-file-pdf"></i> Download CV</a>

<h4>Research Interests</h4>
- *Usable Privacy in IoT Automated Applications on IFTTT tool*
- *IoT Human-Centric Authentication on Earphones and Smart Glasses*
- *Tangible Privacy on Smartphone and Smart Home*

---
<style>
  .pub-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 5px 10;
    margin-bottom: 1em;
    border-bottom: 1px solid #eee;
    position: relative; 
  }

  .pub-info {
    flex: 1;
    padding-right: 25px;
  }

  .pub-abstract-preview {
    flex: 0 0 140px; 
    opacity: 0.7;
    transition: all 0.4s ease;
    z-index: 1;
    display: flex;
    justify-content: flex-end;
  }

  .pub-item:hover .pub-abstract-preview {
    opacity: 1;
  }

  .abstract-link {
    display: block;
    width: 100%;
    text-decoration: none;
  }

  .pub-abstract-preview img {
    width: 100%;
    height: auto;
    border: 1px solid #ddd;
    display: block;
    border-radius: 2px;
    background-color: white; /* Prevents seeing the text behind when zoomed */
    transition: transform 0.4s cubic-bezier(0.165, 0.84, 0.44, 1), box-shadow 0.3s ease;
    backface-visibility: hidden;
    transform-origin: right center; /* Scaling starts from the right edge */
  }

  /* Centering Zoom Effect */
  .pub-abstract-preview:hover img {
    transform: scale(5.5) translateX(-0%); /* Grows and moves to page center */
    box-shadow: 0 15px 40px rgba(0,0,0,0.4);
    border-color: #3498db;
    position: relative;
    z-index: 100;
  }

  .pub-abstract-preview:hover {
    z-index: 100;
    cursor: zoom-in;
  }
</style>

<h4>Publications</h4>
<ul style="list-style-type: none; padding-left: 0;">

  <li class="pub-item">
    <div class="pub-info">
      Romare, Piero. 
      "Dynamic Privacy and the Contextual Calibration of Control for Smartphones in Public Spaces" 
      <em>Moving Beyond Clicks: Rethinking Consent and User Control in the Age of AI (Workshop at CHI ’26)</em>, ACM, 2026.
      <a href="https://pieroromare.github.io/assets/pdf/C009.pdf">[paper]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/positional_paper.png" target="_blank" class="abstract-link">
        <img src="assets/img/positional_paper.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Tjeldflaat, Andreas; Romare, Piero; Onishi, Yuki; Fjeld, Morten;  Sætrevik, Bjørn.
      "A Two-Week In-the-Wild Study of Screen Filters and Camera Sliders for Smartphone Privacy in Public Spaces" 
      <em>In Twentieth International Conference on Tangible, Embedded, and Embodied Interaction (TEI ’26)</em>, ACM, 2026.
      <a href="https://doi.org/10.1145/3731459.3773309">[paper]</a> <a href="https://doi.org/10.48550/arXiv.2602.08465">[preprint]</a> <a href="">[video]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/tangible_privacy.png" target="_blank" class="abstract-link">
        <img src="assets/img/tangible_privacy.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Romare, Piero. 
      "A User-Centric Approach to Usable Privacy for IoT Trigger-Action Platforms." 
      <em>Research Chalmers</em>, Licentiate thesis, Chalmers University of Technology, 2025. 
      <a href="https://research.chalmers.se/publication/544575/file/544575_Fulltext.pdf">[introduction]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/lic.png" target="_blank" class="abstract-link">
        <img src="assets/img/lic.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Romare, Piero; Karegar, Farzaneh; Fischer-Hübner, Simone. 
      "Towards Usable Privacy Management for IoT TAPs: Deriving Privacy Clusters and Preference Profiles" 
      <em>Under submission.</em> 
      <a href="https://doi.org/10.48550/arXiv.2511.11209">[preprint]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/privacy_profile.png" target="_blank" class="abstract-link">
        <img src="assets/img/privacy_profile.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Romare, Piero. "User-Driven Privacy Factors in Trigger-Action Apps: A Comparative Analysis with General IoT." 
      <em>18th IFIP Summer School on Privacy and Identity Management</em>, Springer, 2023. 
      <a href="https://doi.org/10.1007/978-3-031-57978-3_16">[paper]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/literature_review.png" target="_blank" class="abstract-link">
        <img src="assets/img/literature_review.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Romare, Piero; Morel, Victor; Karegar, Farzaneh; Fischer-Hübner, Simone. 
      "Tapping into Privacy: A Study of User Preferences and Concerns on Trigger-Action Platforms." 
      <em>2023 20th Annual International Conference on Privacy, Security and Trust (PST)</em>, 2023. 
      <a href="https://doi.org/10.1109/PST58708.2023.10320180">[paper]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/fc.png" target="_blank" class="abstract-link">
        <img src="assets/img/fc.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>

  <li class="pub-item">
    <div class="pub-info">
      Carlucci, Mattia; Cecconello, Stefano; Conti, Mauro; Romare, Piero. 
      "Eathentication: A Chewing-based Authentication Method." 
      <em>2020 IEEE Conference on Communications and Network Security (CNS)</em>, 2020.
      <br><a href="https://doi.org/10.1109/CNS48642.2020.9162343">[paper] </a><a href="https://patentscope.wipo.int/search/en/detail.jsf?docId=WO2021148932">[patent] </a><a href="https://pieroromare.github.io/assets/video/eathenication_ai_voice.mp4">[video]</a>
    </div>
    <div class="pub-abstract-preview">
      <a href="assets/img/eathentication.png" target="_blank" class="abstract-link">
        <img src="assets/img/eathentication.png" alt="Graphical Abstract">
      </a>
    </div>
  </li>
</ul>


---

<h4>Teaching</h4>
- *Object Oriented Programming* (Chalmers University of Technology, 2024-current)
- *Advanced Programming in Python* (Chalmers University of Technology, 2022-current)
- *Tangible Interaction* (Chalmers University of Technology, 2022-current)
- *Introduction to Programming in Python* (Chalmers University of Technology, 2022-2023)
- *Cognitive, Behaviour and Social Data* (University of Padua, 2021-2022)

---

<h4>Posters and Presentations</h4>

AsiaCCS (Aug 2025) - Hanoi, Vietnam <br>
Mitsubishi Information Technology Research Institute (Oct 2024) - Tokyo, Japan <br>
Meiji University (Oct 2024) - Tokyo, Japan <br>
CISPA Helmholtz Center (Jul 2024) - Saarbrücken, Germany<br>
Lund University (May 2024) - Lund, Sweden<br>
ETH Zürich (May 2024) - Zürich, Switzerland<br>
WASP Winter Conference (Jan 2024) - Norrköping, Sweden<a href="https://internal.wasp-sweden.org/winterconf2024/posters/piero_romare.pdf"> [poster]</a><br>
Chalmers University of Technology (Oct 2023) - Göteborg, Sweden<br>
Massachusetts Institute of Technology (Sept 2023) - Boston, USA<br>
University of Pittsburgh (Sept 2023), Pittsburgh, USA<br>
RISE Stockholm (Sept 2023) - Stockholm, Sweden<br>
Denmark Technical University (Aug 2023) - Copenhagen, Denmark<br>
Oslo University (Aug 2023) - Oslo, Norway<br>
Uppsala University (May 2023) - Uppsala, Sweden<br>
University of Padua (May 2023) - Padua, Italy<br>
Karlstad University (Nov 2022) - Karlstad, Sweden

---
<h1 style="font-size: 0.7em;"> 
  (Infographic generated with NotebookLM)<br>
  (Video translated in English using AI automatic voice translator)
</h1>