---
Title: 'File Paths'
Description: 'A file path describes the location of a file in a web sites folder structure. They are used to link to external files.'
Subjects:
  - 'Web Development'
  - 'Web Design'
Tags:
  - 'File Paths'
  - 'Files'
  - 'URL'
CatalogContent:
  - 'learn-html'
  - 'paths/front-end-engineer-career-path'
---

A file path describes the location of a file in a web site's folder structure. They are used to link to external files, like:

- Websites
- Images
- Videos
- MP3 files
- Style sheets
- JavaScript code

## Absolute File Paths

URL paths in HTML can be absolute paths, like a full URL, for example:

**<span>https\:<span>\/\/codecademy\.com/resources/docs**

```html
<a href="https://www.codecademy.com/resources/docs">
  The URL for this anchor element is an absolute file path.
</a>
```

An example of absolute file path to an image would be as follows. Notice it uses the protocol, domain, and local of the asset to be linked.

**<span>https\:<span>\/\/github\.githubasset\.com/images/modules/logos_page/GitHub-Logo.png**

```html
<a href="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png">
  The URL for this anchor element is an absolute file path.
</a>
```

## Relative File Paths

Relative file path are paths that links to a local file in the same folder or on the same server, for example:

- **./about.html**
- **./style.css**
- **./images/logo.png**

Relative file paths begin with `./` followed by a path to the local file. `./` tells the browser to look for the file path from the current folder.

```html
<a href="./about.html">
  The URL for this anchor element is a relative file path.
</a>
```
Relative file paths can also begin with `../` followed by a path to the local file. `../` tells the browser to look for the file path fromt he **parent** folder.

```html
<a href="../about.html">
  The URL for this anchor element is a relative file path. It goes to the parent folder and access the file about.html
</a>
```

## Link to a Specific Part of the Page

The anchor element `<a>` can create hyperlinks to different parts of the same HTML document using the `href` attribute to point to the desired location with `#` followed by the `id` of the element to link to.

```html
<div>
  <p id="id-of-element-to-link-to">A different part of the page!</p>
</div>
```
<p id="id-of-element-to-link-to">A different part of the page!</p>
Recall that the `id` tag is unique, so any link to an element with this `id` is well defined.  Any element that can be given an  `id` tag can be the target of a relative link. For example, below is an image which is the target of a relative link.

```html
<div>
  <img id="id-of-element-to-link-to-2" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png"/>
</div>
```
<img id="id-of-element-to-link-to-2" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png"/>
<!-- Later in the page --->

<a href="#id-of-element-to-link-to">Take me to a different part of the page</a>

<a href="#id-of-element-to-link-to-2">Take me to the GitHub image</a>
```
