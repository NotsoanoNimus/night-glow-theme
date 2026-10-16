# Night Glow vscode Theme
A semi-nostalgic color theme that draw from the design of [my personal portfolio site](https://xmit.xyz/).


### Color Palette
| Purpose | Color | Notes |
| --- | --- | --- |
| Foreground | <span style="color:#fb9711;">**#fb9711**</span> | |
| Background | <span style="background-color:#999;color:#212121;">**#212121**</span> | |


### How to Develop
- Open this repository in vscode (_CTRL+K_, _CTRL+O_, select the path to the cloned repo).
- Press **F5** to open the _Extension Development Host (EDH)_ in a separate window.
  - This window should immediately apply the theme for you.
- In this window, open up a repository you're interested in viewing.
- Press _CTRL+SHIFT+P_ and start typing `inspect editor tokens`
  - Select `Developer: Inspect Editor Tokens and Scopes`
  - This gives you a better idea of how the theme is applied, whether that's by language-specific styles or from the broad theme styles.
- If at any point the EDH window stops picking up your JSON changes when you save them, just reload the EDH window: _CTRL+SHIFT+P_, type `reload`, and select `Developer: Reload Window`.


### Contributing
While this is a labor of my own love for quiet weekends, I absolutely welcome contributions to the theme. _However_, please be understanding if I'm not willing to accept some stylistic choices, as the theme is very personal to me.

You are more than welcome to maintain your own fork this repository if it comes down to that.


#### Language-specific Contributions
Ensure your entries into the primary JSON file are organized into their own language-specific segment of the `tokenColors` array. They should be well separated from other language-specific styles (to whatever degree they can be).

To begin working on language-specific styles, you can open the scopes inspector (detailed above), click around, and fiddle with the `TextMate scopes` that include your language (typically as a suffix).

For example, `string.quoted.double.include.c` is very specific to the style settings for double-quoted `#include` strings in the C language.

There's probably also a generator available, but I'm too much of a boomer to know where/how.

Anyway, if you submit a Pull Request, please include one or more links to sample projects that your styles can be checked against.


### Misc Docs for Theme-crafting
- `"colors":` keys reference: https://code.visualstudio.com/api/references/theme-color

