---
layout: master
include: workshop

# location and address
# you can also link to a map using e.g. openstreetmap, for example:
# location: "<a https://www.openstreetmap.org/node/1771739362">Teknikringen 14, 11428 Stockholm</a>
location: Online Zoom room

# date and time
time: "9:00 - 17:00"    
dates: "September 22-23, 2020"

# Add link to registration form here and specify when the registration opens and whether it is closed
registration_form: https://indico.neic.no/event/125/
registration_open_date: February 17, 2020
registration_is_closed: false

# names of instructors and helpers
instructors: 
 - Raphaela Heil
 - Thor Wikfeldt
helpers: 
 - TBD

# contact email address
contact: kthw@kth.se

# normally no need to modify this
goals:
    The aim of this course is to demonstrate to and familiarize
    the workshop participants with best practices and tools in modern research
    software development. The main focus is on professional tools
    for efficiently writing and maintaining research software.
    Since most research code is developed in a collaborative
    setting, we will discuss tools and workflows which facilitate
    this process. Most of the content is also relevant to
    a single researcher.

# software that should be installed for the workshop (update if needed)
software:
  - title: Bash
    url: https://coderefinery.github.io/installation/bash/
  - title: Editor
    url: https://coderefinery.github.io/installation/editors/
  - title: Git
    url: https://coderefinery.github.io/installation/git/
  - title: Python
    url: https://coderefinery.github.io/installation/python/
  - title: (optional) Visual diff tools
    url: https://coderefinery.github.io/installation/difftools/
  - title: Accounts
    url: https://coderefinery.github.io/installation/#accounts

# adjust schedule here if needed, and assign lessons to instructors
schedule:
  - date: Day 1
    morning:
      - time: 9:00 - 9:30
        title: Welcome and practical information
        url: https://github.com/coderefinery/workshop-intro/blob/master/README.md
      - time: 9:30 - 12:00
        title: Introduction to version control - part 1/2 
        url: https://coderefinery.github.io/git-intro/
    afternoon:
      - time: 13:00 - 15:00
        title: Introduction to version control - part 2/2
        url: https://coderefinery.github.io/git-intro/
      - time: 15:30 - 17:00
        title: TBD
        url: 
  - date: Day 2
    morning:
      - time: 9:00 - 12:00
        title: Collaborative distributed version control 1/2
        url: https://coderefinery.github.io/git-collaborative/
---