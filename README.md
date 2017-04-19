Vim configuration file for *macOS*

Made from the nice enough [maximum-awesome](https://github.com/square/maximum-awesome) and merging it 
with my original [Linux configuration](https://github.com/mfournialvimLinux).

The result is a very functional Vim environment that benefits from the iTerm2 functions

# Installation
Go to your home directory
`$ cd ~`
Then clone this repository
`$ git clone https://www.github.com/mfournial/vimMac`

If your .vim folder *doesn't exists* yet:
`$ mkdir .vim`
Otherwise, make sure the file that are in your existing directory are not going to conflict with these, in doubt:
`$ mkdir .vimOld`
`$ mv .vim/* .vimOld/`

Now let's move all the files inside the .vim folder
`$ mv vimMac/* .vim/`
`$ rm -r macVim`

But nothing works yet because Vim look for the files in the home directory, let's create some links to solve that problem
`$ ln -s .vimrc .vim/vimrc
ln -s .vimrc.bunldes .vim/vimrc.bundles
ln -s .vimrc.bundles.local .vim/vimrc.bundles.local
ln -s .vimrc.local .vim/vimrc.local`

You should be set!
`$ vi`


# What you can't get out of the box in this repo
## Font
I'm using a nice sleek font called [iosevka](https://github.com/be5invis/Iosevka) that is very thin and
horizontally condensed, which is essential for me
## Lightbar
The cool separators takens from the powerbar plugin for Vim require some work, it's the worse really.
Unless you know how to use Fontpatcher on Mac I recommend the other one they talk about on Lightbar doc,
I used it for Linux without sudo rights and it worked just fine.
## iTerm2
Classic I would say, the default shortcuts work fine with what we already have.

> So many people use Vim and Ruby (was literally in every website I was going through), is Ruby really the best?

# Known bugs and issues
The maximum-awesome integration will fail to update some plugins. It's a git issue that just need a bit of file permissions tweeking will do it if I have time 
