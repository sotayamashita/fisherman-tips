[slack-link]: https://fisherman-wharf.herokuapp.com
[slack-badge]: https://fisherman-wharf.herokuapp.com/badge.svg

[![Slack][slack-badge]][slack-link]

# Fisherman Tips

Translations:

* Japanese: "[🐟 fish-shell と fihserman の tips](http://qiita.com/sotayamashita/items/61d49431053c44f01714)" on Qiita


## Table of Contents

* [Bootstrap](#bootstrap)
* [Test](#test)
* [Migration](#migration)


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

**Migrate from oh-my-fish to fisherman**

1. Just install fisherman
2. If you happen to be also running any fisherman before 2.0 alongside omf
3. Add omf plugin names to ~/.config/fish/fishfile and run fisher
4. Remove omf directories and files

It has been discussed on [Migration instructions from oh-my-fish to fisherman? #223](https://github.com/fisherman/fisherman/issues/223).


## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Sota Yamashita](https://github.com/sotayamashita) has waived all copyright and related or neighboring rights to this work.
