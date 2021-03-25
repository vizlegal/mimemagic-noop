# Mimemagic NOOP

this is a gem with no functionality other them make your bundle dependecy tree work.

any call to mimemagic fill fail, this is just a blank gem!
only use if you don't actually need `mimemagic`

with the removal of old version of https://github.com/minad/mimemagic
some build have become impossible until https://github.com/rails/rails/issues/41750
as been addressed

if you know you are not using activestorage, you can exclude that from bundle
https://gist.github.com/mensfeld/3437de2fae7fc58faccbf28c2e825443

but have depedencies that require `rails` it gets tricky
this is where this gem comes in

add this to your gemfile, to replace minemagic 0.3.5

```
gem "mimemagic", git: "https://github.com/vizlegal/mimemagic-noop"
```
and run

```
bundle update mimemagic
```

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
