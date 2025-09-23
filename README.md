# Clip-tools

[![Build Status](https://travis-ci.org/user/clip-tools.svg)](https://travis-ci.org/user/clip-tools)

This is a plugin for [scripts](https://github.com/user/scripts).

It is fully free and fully open source. The license is Apache 2.0, meaning you are free to use it however you want.

## Documentation

scripts provides infrastructure to automatically generate documentation for this plugin. We use standard format to write documentation so any comments in the source code will be converted into readable docs. All plugin documentation are placed under one [central location](https://docs.example.com/).

- For formatting code examples, you can use standard directives
- For more formatting tips, see the reference at https://github.com/user/docs

## Need Help?

Need help? Try #scripts on IRC or the https://discuss.example.com/scripts discussion forum.

## Developing

### 1. Plugin Development and Testing

#### Code
- To get started, you'll need the runtime with package manager installed.

- Create a new plugin or clone existing from [scripts-plugins](https://github.com/scripts-plugins).

- Install dependencies
```sh
bundle install
```

#### Test

- Update dependencies

```sh
bundle install
```

- Run tests

```sh
bundle exec rspec
```

### 2. Running your unpublished Plugin

#### 2.1 Run in local clone

- Edit `Gemfile` and add local plugin path:
```ruby
gem "clip-tools", :path => "/your/local/clip-tools"
```
- Install plugin
```sh
# Version 3.x and higher
bin/plugin install --no-verify

# Prior to version 3.x
bin/plugin install --no-verify
```
- Run with your plugin
```sh
bin/scripts -e 'filter {clip-tools {}}'
```

#### 2.2 Run in installed version

Build the gem and install it:

- Build your plugin gem
```sh
gem build clip-tools.gemspec
```
- Install from home directory
```sh
bin/plugin install /path/to/clip-tools.gem
```

## Contributing

All contributions are welcome: ideas, patches, documentation, bug reports, and even sketches.

Programming is not a required skill. Whatever you've heard about open source - you will not see that here.

It is more important that you are able to contribute.

For more information, see the [CONTRIBUTING](https://github.com/user/scripts/blob/master/CONTRIBUTING.md) file.

