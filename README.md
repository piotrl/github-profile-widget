# GitHub profile card

Widget shows your profile form GitHub directly on your website!  
Show your current projects always up to date.

![Screenshot](./demo/screenshot.png)

### Main features
- Top languages statistic
- Configurable list of repositories by most starred or last updated
- Amount of followers
- No jQuery and other libraries required


**Live demo at [CodePen](http://codepen.io/piotrl/pen/cwbgJ)**

---

## Download
By bower or just clone repository.
```
bower install github-profile-widget
```
You will find important files in `/dist/` directory.

## Installation

Include script and style inside of your `<head>` tag:
```
<script type="text/javascript" src="gh-profile-widget.js"></script>
<link rel="stylesheet" href="gh-profile-widget.css" />
```

Include HTML tag anywher you would like to place widget: 
```
<div id="github-widget"></div>
```
You can also add attribute data-username with `YOUR_GITHUB_USERNAME`.

```
<div id="github-widget" data-username="YOUR_GITHUB_USERNAME"></div>
```

We are almost done. You only need to init your new widget:

## Configuration
Example of use
```
var githubWidget = new GitHubWidget({
	template: '#github-widget',
	sortBy: 'stars',
	reposHeaderText: 'Most starred',
	maxRepos: 5
});
```

## Configuration options   

Attribute  | Options                   | Default             | Description
---        | ---                       | ---                 | ---
`username` | *string*				   | `null`              | GitHub profile username
`template` | *string*                  | `#github-widget`    | DOM selector of your widget in HTML
`sortBy`   | `stars`, `updateTime`     | `updateTime`        | Repositories sorting method
`maxRepos` | *int*			           | `5`				 | Indicates amount of showed repositories. `0` Shows anything.
`reposHeaderText`     | *string*       | `Last updated repositories`| Text that is shown in labbel above repositories list                           

---

I love feedback, send me one!
- on twitter: [@constjs](https://twitter.com/constjs) 
- create [new issue](https://github.com/piotrl/github-profile-card/issues/new)

Remember no other libraries required. It's like gluten free ;)

![gluten-free](http://forthebadge.com/images/badges/gluten-free.svg)