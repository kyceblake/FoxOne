# Kyle's Firefox theme

Based on Firnschnee/FoxOne tag `3.8.8`. Customizations live on branch `kyle-custom`; the `upstream` remote retains the original project.

- Shared dark palette in both CSS files.
- Hidden address-bar search selector, translate, picture-in-picture, and bookmark buttons.
- Selected tab uses a muted blue background and teal underline.
- Panel and sidebar borders match the desktop palette.

Firefox profile `~/.config/mozilla/firefox/dwp3cvgo.default-esr/chrome/` links to this checkout's `userChrome.css` and `userContent.css`. Edit these files here, commit changes, then restart Firefox. Original installed files remain beside the links as `*.before-local-fork`.

To review upstream updates:

```sh
git fetch upstream --tags
git log --oneline HEAD..upstream/HEAD
```

Merge a chosen upstream version into `kyle-custom`, preserving customizations and resolving any CSS conflicts before restarting Firefox.

GitHub fork: https://github.com/kyceblake/FoxOne. The `origin` remote points to this fork; customizations are published on `kyle-custom`.
