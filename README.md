# Static Boosted

Middleman + Bootstrap + Initializr

- **Middleman** http://middlemanapp.com/
- **Bootstrap** http://getbootstrap.com/
- **Initializr** http://initializr.com/

## Middleman Github Pages

[Github Pages](http://pages.github.com) hosts static sites for free, Middleman Github 
Pages brings the two together. Middleman Github Pages is just a few rake tasks 
that automate the process of deploying a Middleman site to Github Pages.

## Options

You cannot deploy your site if you have uncommitted changes. You can
override this with the `ALLOW_DIRTY` option:

```shell
bundle exec rake publish ALLOW_DIRTY=true
```

You can append a custom suffix to commit messages on the build branch:

```shell
bundle exec rake publish COMMIT_MESSAGE_SUFFIX="--skip-ci"
```

You can change the remote that you deploy to:

```shell
bundle exec rake publish REMOTE_NAME=upstream
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
