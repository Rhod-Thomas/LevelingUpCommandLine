https://www.redhat.com/en/blog/fzf-linux-fuzzy-finder
All following learnings from the above source. 


fzf is an interactive search. The power of it is evident from just typing fzf. 

But, its output is printed into standard output so you can do incredible things like this:

vim $(fzf)
cp $(fzf) ~/.config/pipewire

Preview the file contents like this (you can also make the preview smarter with scripts):
fzf --preview 'batcat --color=always {}'

Set these options as defaults in .bashrc like so:
export FZF_DEFAULT_OPTS="--preview 'batcat --color=always {}'" 

