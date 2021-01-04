

# scripts

A Git repository to provide some useful scripts.


## Usage

Clone the repository:

```bash
cd ~
mkdir -p bin
git clone --bare https://github.com/xengineering/scripts.git
git --git-dir=$HOME/scripts.git/ --work-tree=$HOME/bin/ checkout
```

Add alias for repository handling and PATH extension to .bashrc. You can skip this point if you also use my [dotfiles project](https://github.com/xengineering/dotfiles):

```bash
echo "alias scripts='/usr/bin/git --git-dir=$HOME/scripts.git/ --work-tree=$HOME/bin/'" >> ~/.bashrc
echo "PATH=$PATH:~/bin" >> ~/.bashrc
```

Update the scripts repository on demand:

```bash
scripts pull
```

