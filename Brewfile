cask_args appdir: '/Applications'

brew 'git'

brew 'libgit2'

brew 'imagemagick'

# To do
# - install mysql

# Testing
brew 'qt@5.5' if MacOS::Xcode.installed?

# https://github.com/ggreer/the_silver_searcher
brew 'the_silver_searcher'

tap 'homebrew/services'

brew 'postgresql'

brew 'mysql'

brew 'redis'

brew 'phantomjs'

brew 'hub'

cask 'github-desktop'

if ! app_is_installed 'virtualbox'; then
  cask 'virtualbox'
fi

if ! app_is_installed 'vagrant'; then
  cask 'vagrant'
fi

if ! app_is_installed 'vagrant-manager'; then
  cask 'vagrant-manager'
fi

if ! app_is_installed 'slack'; then
  cask 'slack'
fi

if ! app_is_installed 'sublime-text'; then
  cask 'sublime-text'
fi

fancy_echo "Update heroku binary..."
brew unlink heroku
brew link --force heroku
