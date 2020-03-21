# Tech Talks Web
South City Resident's Group for hands-on technical meetup

[![Website Status](https://img.shields.io/website?url=https%3A%2F%2Ftech-talks-sc.netlify.com&logo=circle&logoColor=white)](https://tech-talks-sc.netlify.com/)

[![Netlify Status](https://api.netlify.com/api/v1/badges/8c17908c-238c-4924-a825-d300a48661cd/deploy-status)](https://app.netlify.com/sites/tech-talks-sc/deploys)


## Requirements

1. Hugo Extended [Download](https://github.com/gohugoio/hugo/releases)

## Update Theme Repo

```
git submodule init
git submodule update
```

> Theme repo is added as a `git submodule`

## Development Server

```
hugo serve
```

## Content Editing

Create new meetup

```
hugo new meetups/south-city-tech-talks-meetup-October-2019.md
```

Edit existing pages or posts

```
Inspect content/
```

## Hugo Usage

```
Congratulations! Your new Hugo site is created in /home/user1/Work/dev/tech-talks-web.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/, or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
```
