# Port Hope HBIA Website

Website by Riley Ashton.

Based off template by [Darin Dimitroff](https://twitter.com/deezel), [spacefarm.digital](https://www.spacefarm.digital).

## Architecture

- Hugo static site generator
- Decap CMS (with Netlify Identity) for content managment
- CSS3 (vanilla)
- glide.js for image sliding (locally hosted minified js and css)
- no npm, no webpack, no transpiler, etc

## Local Development

Install hugo and run `hugo server` for a hot reloading server on port 1313.

## Layouts

The template is based on small, content-agnostic partials that can be mixed and matched. The pre-built pages showcase
just a few of the possible combinations. Refer to the `site/layouts/partials` folder for all available partials.

## CSS

Vanilla CSS3, mostly in /static/styles.css. Inline styles are fine.

## SVG Social Icons

The social media icons are in `site/assets/img`.
Make sure you use consistent icons in terms of viewport and art direction for optimal results.
For an icon named `icons-facebook.svg`, refer to the SVG `social-icon` partial like so:

```
{{ partial "social-icon" (dict "link" "#" "svg" "icons-facebook" "alt" "Kaldi on Facebook") }}
```

## Getting started

Use the deploy button to setup on netlify.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/decaporg/one-click-hugo-cms&stack=cms)

This will setup everything needed for running the CMS:

* A new repository in your GitHub account with the code
* Full Continuous Deployment to Netlify's global CDN network
* Control users and access with Netlify Identity
* Manage content with Decap CMS

Once the initial build finishes, you can invite yourself as a user. Go to the Identity tab in your new site, click "
Invite" and send yourself an invite.

Now you're all set, and you can start editing content!

