# dotfiles

install git 
install stow 
clone this repo in your home directory
run command "stow ."


https://nixos.org/download/
https://github.com/DeterminateSystems/nix-installer
https://nix-community.github.io/home-manager/index.xhtml#ch-introduction
https://search.nixos.org/packages?channel=24.05&show=tmux&from=0&size=50&sort=relevance&type=packages&query=tmux
https://nixos.wiki/wiki/Flakes
https://www.youtube.com/watch?v=hLxyENmWZSQ&t=16s

sh <(curl -L https://nixos.org/nix/install) --no-daemon
export NIXPKGS_ALLOW_UNFREE=1
nix shell nixpkgs#home-manager --extra-experimental-features "nix-command flakes" --impure
home-manager switch --flake .#dimi --extra-experimental-features "nix-command flakes" --impure
