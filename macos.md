### Over-essential
```shell
# run xcode-select --install
xcode-select --install
# install homebrew
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/<User>/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
# install git
brew install git
# install oh my zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Essential
```shell
echo 'install slack'
brew install --cask slack &
wait $!

echo 'install vscode'
brew install --cask visual-studio-code &
wait $!

echo 'install zoom'
brew install --cask zoom &
wait $!

echo 'install postman'
brew install --cask postman &
wait $!

echo 'install docker'
brew install --cask docker &
wait $!

echo 'install node.js'
brew install node &
wait $!

echo 'install charles proxy'
brew install --cask charles
wait $!

echo 'install github cli'
brew install gh
wait $!

echo 'install gitmoji'
brew install gitmoji
wait $!

echo 'install peco filter'
brew install peco
wait $!

echo 'install midnight commander'
brew install mc
wait $!

echo done
```
