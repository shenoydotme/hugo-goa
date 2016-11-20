# Goa

Goa is a clean, simple and minimalist theme for blogs and personal websites.

<img src="http://i.imgur.com/vqMd1Mx.png" width="40%" height="40%" />

## Demo

You can find the demo site in action [here](https://shenoybr.github.io/hugo-goa-demo) and the source [here](https://github.com/shenoybr/hugo-goa-demo).

## Installation

From the root of your blog:

```
mkdir -p themes
cd themes
git clone https://github.com/shenoybr/hugo-goa 
```

## Content creation

### Creating a post

To create a new page or post:

````
hugo new about.md
````
or

````
hugo new posts/first.md
````

You can now go ahead an edit the newly created file under the `content` directory. Once you are finished editing, to have hugo generate the page, set `draft = false` in the articles front matter. 

### Organizing pages

The above example demonstrates how to create a pages and posts. Hugo automatically applies the list templates for a directory of pages/posts, which works well for blogs and posts. However, you may want at times want to override this behavior and create a standalone page (like an about page or projects page) or have more control of what content is listed from within the directory. In such cases, you can override the default behavior by placing an index.md file in the corresponding content
directory.

````
hugo new projects/index.md
````

### Page settings

These settings are at the page level.

- `showpagemeta`: default=`true`. This allows you to disable page meta information from being displayed. For example, this setting is disabled [here](https://shenoybr.github.io/hugo-goa-demo/about/) and enabled [here](https://shenoybr.github.io/hugo-goa-demo/coderag/).
- `showcomments`: default=`true`. Enables or disable comments. For example, this setting is disabled [here](https://shenoybr.github.io/hugo-goa-demo/blog/third/) and enabled [here](https://shenoybr.github.io/hugo-goa-demo/blog/first/).

## Configuration

The provided [config.toml](https://github.com/shenoybr/hugo-goa/blob/master/exampleSite/config.toml) describes all options and features that are supported. Configure it your way!

### Basic Configuration

These are site wide configuration parameters that are used by this template.

- `baseurl`: This is the root of your site.
- `builddrafts`: default=`false`. Enables or Disable building drafts when hugo is run.
- `canonifyurls`: default=`false`. Prefix all relative URLs with your base URL. [More Information](https://gohugo.io/extras/urls#canonicalization).
- `languageCode`: Used to set site localization preferences. eg. `en-US`.
- `contentdir`: Where hugo can find your content. eg. `content`.
- `layoutdir`: Where hugo can find your templates. eg. `layouts`.
- `publishdir`: Where hugo generates the static site. eg. `public`.
- `author`: Site author name. eg. `Erlich Bachman`.
- `title`: Site title name. eg. `Erlich Bachman`.
- `theme`: Your theme name should be set to `hugo-goa` if using this theme.

## Hugo Built-in Features

These are features that hugo provides and are used by this template.

- `disqusShortname`: Your discusShortname if you want to enable comments on your posts.
- `googleAnalytics`: Your google analytics id for tracking.
- `enableRobotsTXT`: Enable or disable search engines from crawling your site.

## Site Settings `[params]`

These are settings that are specific to this theme.

- `author`: Main author name. eg. `Erlich Bachman`.
- `intro`: Author introduction. This field supports markdown. eg. `Startup Guru Extraordinaire`.
- `description`: Author description. This field supports markdown. eg. `Now @Pied Piper. Previously @Hacker Hostel, @Bachmanity and @Aviato. <br/> \"What is F times 5? It's Fleventy-five.\"`.
- `authorimage`: Location of author image under static/img directory. eg. `headshot.jpg`
- `dateformat`: Golang date format to be used on this site. eg. `Jan 2, 2006`

### Site Meta Settings `[params.meta]`

These settings are included in the site's meta section.

- `description`: User this field to describe your site to search engines. eg. `Simple minimalist theme`.
- `keywords`: Keywords that desribe your site. eg. `minimalist,blog,goa,hugo,developer`.

### Social Accounts `[params.social]`

These settings to display your social accounts.

- `github`: Your github username.
- `instagram`: Your instagram username.
- `linkedin`: Your linkedIn username.
- `twitter`: Your twitter username.
- `facebook`: Your facebook username.
- `google`: Your google username.
- `email`: Your email.

### Extras `[params.extra]`

These settings for extra features that this site uses.

- `copyright`: Add a copyright statement to the bottom of the theme. eg. `© 2016. Erlich Bachman. [Some Rights Reserved](http://creativecommons.org/licenses/by/3.0/)."`
- `poweredby`: Help promote this theme and give the authors credit. eg. `true` or `false`.
- `highlightjs`: Use highlightJS to highlight code on your site. eg. `true` or `false`.

### Main Menu `[[menu.main]]`

These settings for the main menu that is displayed on the home page.

- `name`: Name of menu item. eg. `blog`
- `weight`: Weight of this menu item. Higher items go to the bottom. eg. `100`
- `url`: Root URL for this section/page. eg. `/blog/`.

Example:
```
[[menu.main]]
    name = "blog"
    weight = 100
    url = "/blog/"
[[menu.main]]
    name = "about"
    weight = 200
    url = "/about/"
[[menu.main]]
    name = "coderag"
    weight = 300
    url = "/coderag/"
```

## Features

* Responsive
* Minimalist
* Bootstrap 3
* Fontawesome
* HighlighJS
* Disqus support for commenting
* Built-in support for 404 pages, Disqus comments and Google Analytics.

## Screenshots

<img src="http://i.imgur.com/vqMd1Mx.png" width="30%" height="30%" />
<img src="http://i.imgur.com/dfj8MHz.png" width="30%" height="30%" />
<img src="http://i.imgur.com/mMFfkZY.png" width="30%" height="30%" />
<img src="http://i.imgur.com/7e67ypn.png" width="30%" height="30%" />
<img src="http://i.imgur.com/lz3RGH9.png" width="30%" height="30%" />
<img src="http://i.imgur.com/IPggNGk.png" width="30%" height="30%" />
<img src="http://i.imgur.com/FW1Bdln.png" width="10%" height="10%" />
<img src="http://i.imgur.com/vTY5GeX.png" width="10%" height="10%" />
<img src="http://i.imgur.com/aJZQYZ6.png" width="10%" height="10%" />
<img src="http://i.imgur.com/rGQJAF3.png" width="10%" height="10%" />

## Contributing

### Bug Reports

1. Search Github Issues to see if the bug has been previously filed.
2. If it has been filed, +1 the post. This helps us in assessing impact and priortitizing the bug.
3. If not previously filed, open a new Github Issue and describe in detail. Attach error traces and provide relavant details to help us solve it.
4. For Hugo issues, search the Hugo [Forum](https://discuss.gohugo.io/)

### Feature Requests

1. Search Github Issues to see if the feature has been previously requested.
2. If it has been filed, +1 the post. This helps us in assessing popularity and priortitizing the feature.
3. If not previously filed, open a new Github Issue and describe it in detail.

### Pull Requests

1. Clone the repository, create the feature/bug branch.
2. Code.
3. Make sure your code follows the style of the project.
4. Test it thoroughly.
5. Open a PR requesting for it to be merged.
6. Describe the feature or issue your are solving in detail. 
7. Wait for its approval.
8. Merge and Rejoice.

## Attribution

The theme's design was inspired by many blogs and themes:

1. Bruno de Carvalho's [blog](http://biasedbit.com).
2. [Hugo Cocoa](http://themes.gohugo.io/cocoa/).
3. [Hugo Vec](http://themes.gohugo.io/hugo-theme-vec/).
4. [Hugo Agency](http://themes.gohugo.io/hugo-agency/).

## License

Licensed under the [MIT](https://opensource.org/licenses/MIT) License. See the [LICENSE](https://raw.githubusercontent.com/shenoybr/hugo-goa/master/LICENSE) file for more details.

