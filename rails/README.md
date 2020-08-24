# Rails

Best practices in Rails applications.

## Background Jobs

- Define a `PRIORITY` constant at the top of delayed job classes.
- Define two public methods: `self.enqueue` and `perform`.
- Put delayed job classes in `app/jobs`.

## Ruby

### Version management

* Use [rbenv](https://github.com/sstephenson/rbenv) to manage multiple ruby versions in your development environment.

* Use a `.ruby-version` file in the project root directory to specify the Ruby version and patch level to be used.
* Include the ruby engine used, eg: `ruby-2.7.1` for mri/yarv ruby 2.7.1
* Do not add `.ruby-version` to `.gitignore`

### Code style and quality

* Use [RuboCop](https://github.com/bbatsov/rubocop) to check your code against style conventions and best practices.

* Use [RubyCritic](https://github.com/whitesmith/rubycritic) to detect and report code smells.
