# url-to-clip

`url-to-clip` is a simple script which presents a simple GUI prompting you to copy an URL. It can be registered as the default browser, allowing you to make an informed choice whenever an application invokes an URL.

I made this because I got fed-up with programs opening random URLs in my browser without confirmation. I prefer using private windows to visit new websites, but all URLs which are opened by default are opened in a normal window.

## Requirements

* zenity - GUI prompt
* fish - since the script is witten in fish script
* xclip - copy URL to clipboard
* sed - for escaping `&` in URLs (the GUI can't handle that verbatim)

## Installation

1. Copy `url-to-clip` to a directory in your `$PATH` (use `/usr/bin` if unsure)
2. Copy `url-to-clip.desktop` to `/usr/share/applications`
3. Change the default browser to `URL to Clip Handler` in your desktop environment
