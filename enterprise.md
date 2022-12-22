# Home

Welcome to the documentation website I built for you. It's mostly bare-bones at the moment, but I'm willing to add features you need.

The way it was designed was to be quick, free, and easy to manage. These documentation pages are written in Markdown, stored on a GitHub repository. To take a look at all the Markdown features this website supports, take a look at [the Elements page](/enterprise/markdown/elements). 

Directory structure and configuration is done in a very easy syntax called YAML. Here's an example:

```yaml
- displayName: Enterprise
  description: A complete package that handles your route, scheduling, recurring billing, and customer management.
  displayIcon: https://www.wisesoftwareinc.com/wp-content/uploads/2021/07/Enterprise-e1626300075144-150x150.png
  pages:
    Markup:
    - Elements
    - Another Page
  
    Sample 1:
    - Test
  
- displayName: Retail
  description: Modern register software designed to make retailers more efficient.
  displayIcon: https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/1200px-Google_2015_logo.svg.png
  pages:
    Test:
      - Hello
```

Merry Christmas!
