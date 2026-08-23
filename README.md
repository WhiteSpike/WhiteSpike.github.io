# WhiteSpike.github.io

# Prerequisites for Development

## [Jekyll](https://jekyllrb.com/docs/installation/):

- [Ruby](https://www.ruby-lang.org/en/downloads/) version 2.7.0 or higher, including all development headers (check your Ruby version using ``ruby -v``)
- [RubyGems](https://rubygems.org/pages/download) (check your Gems version using ``gem -v``)
- [GCC](https://gcc.gnu.org/install/) and [Make](https://www.gnu.org/software/make/) (check versions using ``gcc -v``,``g++ -v``, and ``make -v``)
    - For Windows users, [WinLibs](https://winlibs.com/) contains these two tools.
        - Instead of ``make -v``, you will use ``mingw32-make -v``. You can decide to put it under an alias later.

## Gems:

- You have to install the gems listed in the ``Gemfile`` file through ``gem install <name>``

# Running locally
- Open command prompt in the root folder of the repository and run ``jekyll serve``.
    - This can error if you do not have the required Ruby gems listed in ``Gemfile`` file installed locally.

- Once confirmed the server is running, you can access it through the address listed in ``Server address: ``
    - You will use this to check changes made in the files before commiting to the repository.
    - Alternatively, you can also use ``localhost`` in place of the IP address. (e.g ``localhost:4000``)

# Running through Github Pages

- Once changes are made and committed to the ``release`` branch, a Github Action is triggered which attempts to build and deploy the page through Jekyll workflow.
    - If it fails, review and correction of the latest failed commit is required to ensure correctness.

# Attributions
- Nared's [portfolio repository](https://github.com/naren200/naren200.github.io) used as base for understanding HTML/CSS/Jekyll