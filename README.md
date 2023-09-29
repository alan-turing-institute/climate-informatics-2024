## Welcome!

This is the GitHub repository for Climate Informatics 2024

This repository hosts the code for [Climate Informatics 2024 website](https://alan-turing-institute.github.io/climate-informatics-2024/) and project management for delivery of the conference.

Below we provide basic info and links to more information. 

### Who are we?

We are ...

### What are we doing?

We are organizing ...

### Get involved

All information is available on ...

### Contact us

Feel free to ...


---

### Credit
Based on the [OSR 2020](https://ohbm.github.io/osr2020) and [OSR 2023](https://ohbm.github.io/osr2020) websites. Built using the [Beautiful Jekyll](https://deanattali.com/beautiful-jekyll/) theme by [Dean Attali](https://deanattali.com/).


#### Instructions for building website (these must be run prior to uploading onto GH)
Check the speaker/volunteer CSV files are in place (in _data/speakers, _data/volunteers)
Wipe the built directories if they already exist, and re-build: 
`rm -r _speakers _volunteers; bundle exec jekyll pagemaster speakers volunteers`
Commit the new directories and push the site. This must be done every time the CSV files are changed. 
