---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 20

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Postdoctoral Research Scholar, Astrophysics
    company: University of California, Davis
    company_url: ''
    company_logo: uc-davis
    location: California
    date_start: '2019-07-01'
    date_end: ''
    description: |2-
        I am currently a postdoc in Professor Lloyd Knox's group at UC Davis. I am a member of the *South Pole Telescope* (*SPT*) and *BICEP / Keck* (*BK*) collaborations. Some of my projects have been:
        
        * Developed a hierarchical Bayesian analysis pipeline for the analysis *SPT* and *BK* data (using Julia, `CUDA.jl`, and autodiff). 
        * Built a variational autoencoder model of Galactic foregrounds to capture non-Gaussian behavior (using Python and Tensorflow) [[1]](publication/a-generative-model-of-galactic-dust-emission-using-variational-inference).
        * Developed `v3.0` of [`PySM`](project/example) in collaboration with the Pan-Experiment Galactic science group. Targeted development for performance in HPC environments, and implemented new foreground models using data released since 2016 `v2.0` [[2]](publication/the-python-sky-model-3-software).

  - title: Visiting Doctoral Researcher, Astrophysics
    company: Princeton University
    company_url: ''
    company_logo: princeton
    location: New Jersey
    date_start: '2017-09-01'
    date_end: '2019-06-23'
    description: |2-
        Conducted thesis research under the supervision of Professor Jo Dunkley. Some of my projects were: 
    
        * Used *Planck* data to estimate the foreground contamination of the *ACT* survey. Contributed this to the analysis presented in these papers [[3](publication/the-atacama-cosmology-telescope-dr4-maps-and-cosmological-parameters), [4](publication/the-international-school-for-advanced-studies-sissa-find-out-more-the-atacama-cosmology-telescope-a-measurement-of-the-cosmic-microwave-background-power-spectra-at-98-and-150-ghz)].   
        * Wrote a pixel-fitting likelihood code to forecast the sensitivity of the *Simons Observatory* to spatial variation of foreground frequency dependence [[5]](publication/the-simons-observatory-science-goals-and-forecasts).
    
  - title: Visiting Doctoral Researcher, Astrophysics
    company: University of Tokyo
    company_url: ''
    company_logo: the-university-of-tokyo-logo-vector
    location: Tokyo
    date_start: '2016-08-01'
    date_end: '2017-09-01'
    description: Conducted thesis research under the supervision of Professors Nobuhiko Katayama and Eiichiro Komatsu. I forecasted how we may use space-based laser interferometers and CMB experiments to constrain parity-breaking models of inflation [[6]](/publication/finding-the-chiral-gravitational-wave-background-of-an-axion-su-2-inflationary-model-using-cmb-observations-and-laser-interferometers).
    
  - title: Graduate Student, Astrophysics (PhD)
    company: University of Oxford
    company_url: ''
    company_logo: university-of-oxford-logo
    location: Oxford
    date_start: '2015-10-01'
    date_end: '2016-08-01'
    description: Conducted thesis research under the supervision of Professor Jo Dunkley. I worked primarily on developing the codebase and modeling for the original [`PySM`](project/example) code [[7]](publication/the-python-sky-model-software-for-simulating-the-galactic-microwave-sky), as well as its application in a forecasting project for component separation in future CMB experiments [[8]](publication/simulated-forecasts-for-primordial-b-mode-searches-in-ground-based-experiments).

design:
  columns: '2'
---
