# TAU Group Website

## Installation


### Clone the repo using SSH or Https clone command

> git clone git@github.com:taugroup/taugroup.github.io.git

or
> git clone https://github.com/taugroup/taugroup.github.io.git 
  

### Change directory to taugroup.github.io

> cd taugroup.github.io

### Install [jekyll](https://jekyllrb.com/docs/installation/) if not installed previously
> gem install bundler jekyll

### Run the jekyll server
> bundle exec jekyll serve

### Visit [http://localhost:4000/](http://localhost:4000/) to see the website

## Deployment

[https://jekyllrb.com/docs/continuous-integration/github-actions/](https://jekyllrb.com/docs/continuous-integration/github-actions/)

## Data
To add/modify the data make changes in the **_data** folder in the relevant file.

Use the following format, feel free to make changes
 #### Team Members : team_members.yml file
 
```
- name: Team Member Name
- photo: team_member.png
- info: Some information about the team member
- email: member@team.com
- number_educ: 3
- education1: PhD. in Computer Science
- education2: Contributor to ML Group at TAU Group
- education3: Intel University Ambassador and TAMUD Campus Champion at Texas A&M University

``` 

#### Publications list: publist.yml
```
- title: "Publication title"
  image: publication image.png
  description: Some description about the publications.
  authors: Author1, author2, author3, author4.
  link: 
   url: https://some_url.com
   display: Url_display_title
  news2: News about the publications.
```

#### News List: news.yml
```
- date: 9. January 2022
  headline: "Headline **highlighted text inside**"
```
