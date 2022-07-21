# devenv

🍭 Configuration of my local development environment.

❗️ This is my personal configuration.
Please be attentive if you are going to reuse it.
Before applying this configuration, check it carefully and make sure it won't cause damage to your system.

📝 If you see that something could be improved, don't hesitate to offer a pull request.

## How to apply

### Brew
1. Install brew:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
2. Install development tools and applications:
```bash
brew bundle --file ./Brewfile.work
```
3. Install applications used for personal needs:
```bash
brew bundle --file ./Brewfile.home
```

### iTerm2 profile
1. Profile -> Edit Profiles -> Other Actions -> Import JSON Profiles...
2. Choose the file `iterm.default.profile.json` from this repo.

### Fish
1. Make `fish` the default shell:

```bash
echo /opt/homebrew/bin/fish | sudo tee -a /etc/shells
chsh -s /opt/homebrew/bin/fish
```

2. Add fish paths and configs:

```fish
fish_add_path /opt/homebrew/bin
```


