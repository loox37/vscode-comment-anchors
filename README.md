# Comment Anchors

Place anchors within comments or string to place bookmarks within the context of your code. Anchors can be used to build a simple navigation, making it easier to navigate large files.

## Changelog
View the changelog [here](CHANGELOG.md)

## Features

* Place anchors in comments, strings, documentation, etc.
* Anchors can be viewed in the anchor sidebar view in the activity bar.
* Anchor names, icon colors, and highlight colors can be customized.
* Click an anchor in the sidebar view to scroll it into view. 

## Usage

The default settings come with anchors for the following tags:

* ANCHOR
* TODO
* FIXME
* STUB
* NOTE
* REVIEW

In order to make an anchor, simply place the tag name in a string or comment, with an additional anchor message behind it.

![Preview](media/preview.gif)

All anchor tags have their own color, which can be customized in the settings.

![All tags](media/all-anchors.png);

##Configuration

Use `commentAnchors.parseDelay` to alter the delay in milliseconds between when you stop with typing and when the anchor parser starts. Increasing this value can result in better performance. (Default 200)

```
{
	"commentAnchors.parseDelay": 200
}
```

Use `commentAnchors.tagHighlights.enabled` to set whether tags are highlighted. (Default true)

```
{
	"commentAnchors.tagHighlights.enabled": true
}
```

Use `commentAnchors.tags` to configure the anchor tags. Each tag requires a `name`, `iconColor` and `highlightColor`.

```
"commentAnchors.tags": [
    {
      "tag": "ANCHOR",
      "iconColor": "default",
      "highlightColor": "#A8C023"
    }
]
```

## Issues

Issues can be submitted in the GitHub repository [here](https://github.com/ExodiusStudios/vscode-comment-anchors/issues)

## Contribution

You can contribute to comment-anchors by forking the GitHub [repository](https://github.com/ExodiusStudios/vscode-comment-anchors) and submitting pull requests.

#### Thanks for using Comment Anchors!