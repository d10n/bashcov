# Bashcov [![Build Status](https://secure.travis-ci.org/infertux/bashcov.png?branch=master)](https://travis-ci.org/infertux/bashcov) [![Dependency Status](https://gemnasium.com/infertux/bashcov.png)](https://gemnasium.com/infertux/bashcov) [![Code Climate](https://codeclimate.com/github/infertux/bashcov.png)](https://codeclimate.com/github/infertux/bashcov)

**Code coverage for Bash**

  * [Source Code]
  * [Bug Tracker]
  * [API Documentation]
  * [Changelog]
  * [Rubygem]
  * [Continuous Integration]
  * [Dependencies]
  * [SimpleCov]

[Source Code]: https://github.com/infertux/bashcov "Source Code on Github"
[Bug Tracker]: https://github.com/infertux/bashcov/issues "Bug Tracker on Github"
[API documentation]: http://rubydoc.info/gems/bashcov/frames "API Documentation on Rubydoc"
[Changelog]: https://github.com/infertux/bashcov/blob/master/CHANGELOG.md "Project Changelog"
[Rubygem]: https://rubygems.org/gems/bashcov "Bashcov on Rubygems"
[Continuous Integration]: https://travis-ci.org/infertux/bashcov "Bashcov on Travis-CI"
[Dependencies]: https://gemnasium.com/infertux/bashcov "Bashcov dependencies on Gemnasium"
[Bashcov]: https://github.com/infertux/bashcov
[SimpleCov]: https://github.com/colszowka/simplecov "Bashcov is backed by SimpleCov to generate awesome coverage report"

You should check out the **[demo](http://infertux.github.com/bashcov/test_app/)** -- it's worth a thousand words.

## Installation

`$ gem install bashcov`

## Usage

`bashcov --help` prints all available options.
Here are some examples:

    bashcov ./script.sh
    bashcov --skip-uncovered ./script.sh
    bashcov -- ./script.sh --some --flags
    bashcov --skip-uncovered -- ./script.sh --some --flags

`script.sh` can be a mere Bash script or typically your CI script.
Bashcov will keep track of all executed scripts.

Then it will create a directory named `./coverage/` containing nice HTML files.
Open `./coverage/index.html` to browse the coverage report.

### SimpleCov integration

You can take great advantage of [SimpleCov] by adding a `.simplecov` file in your project's root (like [this](https://github.com/infertux/bashcov/blob/master/spec/test_app/.simplecov)).
See [SimpleCov README](https://github.com/colszowka/simplecov#readme) for more information.

## Contributing

Bug reports and patches are most welcome.
See the [contribution guidelines](https://github.com/infertux/bashcov/blob/master/CONTRIBUTING.md).

## License

MIT
