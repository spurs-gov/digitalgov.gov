<h1><img src="https://demo.digital.gov/img/digitalgov-logo-black.svg" alt="Digital.gov Logo"/></h1>

## We help people in government build better digital services
https://digital.gov

- Sign-up for the [Digital.gov newsletter »]({{< ref "/about/subscribe.md" >}})
- Follow us on [Twitter »](https://twitter.com/digital_gov/)
- Like our page on [Facebook »](https://www.facebook.com/digitalgov/)

Want to learn more about how we work? [Check out our Wiki page »](https://github.com/GSA/digitalgov.gov/wiki)


---


[![CircleCI](https://circleci.com/gh/GSA/digitalgov.gov/tree/master.svg?style=svg)](https://circleci.com/gh/GSA/digitalgov.gov/tree/master)

## Development Guide

[Digital.gov](https://digital.gov/) is built with [Hugo](https://gohugo.io/) and hosted by [Federalist](https://federalist.18f.gov/) and [Cloud.gov](https://cloud.gov/).


### Install NPM Dependencies

`npm install`

### Install Hugo

[Read the HUGO quickstart guide »](https://gohugo.io/getting-started/quick-start/)

**For OSX:**
`brew install hugo`
_see https://gohugo.io/getting-started/installing/ for other OSs_

#### Run

`hugo serve` _(can take 30 secs to launch)_
or
`hugo serve --config=config_dev.yml` _(can take 5 secs to launch but only builds a portion of the content)_

**visit** http://localhost:1313/

#### Test

To run web accessibility testing do the following:  
a. Start a server by following the `Install` and `Run` instructions above. *Site must be running locally to perform the scan.*  
b. At the command line run `npm run test:pa11y` to initiate the accessibility checker.

*Note*: Currently, this only runs accessiblity checks on the site home page as a Proof of Concept demonstration.

Accessibility testing configuration is located in the .pa11yci file. 

We follow the WCAG2AA standard. For more info on the rules being tested checkout the [pa11y wiki](https://github.com/pa11y/pa11y/wiki/HTML-CodeSniffer-Rules).