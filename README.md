[slack-link]: https://fisherman-wharf.herokuapp.com
[slack-badge]: https://fisherman-wharf.herokuapp.com/badge.svg

[![Slack][slack-badge]][slack-link]

# Fisherman Links

## Bootstrap

```fish
# Ensure fisherman and plugins are installed
if not test -f $HOME/.config/fish/functions/fisher.fish
  echo "==> Fisherman not found.  Installing."
  curl -sLo ~/.config/fish/functions/fisher.fish --create-dirs git.io/fisher
  fisher -v
end
```

## Test

**Test if completion works** by [@Markcial](https://github.com/Markcial)

```fish
TEST "Should return ask-pass param" complete -C"foo --ask-p" = "foo --ask-pass" end`
```

## Migration

* [Migration instructions from oh-my-fish to fisherman? #223](https://github.com/fisherman/fisherman/issues/223)

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Sota Yamashita](https://github.com/sotayamashita) has waived all copyright and related or neighboring rights to this work.
