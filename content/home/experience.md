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
  - title: Postdoctoral Research Scholar
    company: University of California, Davis
    company_url: ''
    company_logo: uc-davis
    location: California
    date_start: '2019-07-01'
    date_end: ''
    description: |2-
        Responsibilities include:
        
        * Analysing
        * Modelling
        * Deploying

  - title: Visiting Doctoral Researcher
    company: Princeton University
    company_url: ''
    company_logo: princeton
    location: New Jersey
    date_start: '2017-09-01'
    date_end: '2019-06-23'
    description: |2-
        Conducted thesis research under supervision of Professor Jo Dunkley. Projects included: 
    
        * Using *Planck* data to estimate the foreground contamination of the *ACT* survey. 
        * Writing a pixel-fitting likelihood code to forecast the sensitivity of *Simons Observatory* to spatial variation of foreground frequency dependence. 
    
  - title: Visiting Doctoral Researcher
    company: University of Tokyo
    company_url: ''
    company_logo: the-university-of-tokyo-logo-vector
    location: Tokyo
    date_start: '2016-08-01'
    date_end: '2017-09-01'
    description: Conducted thesis research under supervision of Professor {{< icon name="terminal" pack="fas" >}} Nobuhiko Katayama and Professor Eiichiro Komatsu. I worked mainly on deriving the observational signatures of an axion-SU(2) model for inflation, leading to a [paper](/publication/finding-the-chiral-gravitational-wave-background-of-an-axion-su-2-inflationary-model-using-cmb-observations-and-laser-interferometers) on the topic.
    
  - title: Graduate Student (PhD)
    company: University of Oxford
    company_url: ''
    company_logo: university-of-oxford-logo
    location: Oxford
    date_start: '2015-10-01'
    date_end: '2016-08-01'
    description: Conducted thesis research under supervision of Professor Jo Dunkley. I worked primarily on the original [PySM](/publication/example) code.

design:
  columns: '2'
---
