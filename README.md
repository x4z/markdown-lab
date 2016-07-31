
# Markdown Lab

This lab aims to easier the building of the markdown environment for slides, books, resume and articles.

## Download

    $ git clone https://github.com/tinyclub/markdown-lab.git
    $ cd markdown-lab/

## Installation

To install the necessary tools, try `tools/install-local-lab.sh` for local
machine and `tools/install-docker-lab.sh` for virtual machine.

For docker machine, need to open it with `tools/run-docker-lab-daemon.sh` and
login `http://localhost:6080/vnc.html` in with `ubuntu` password.

## Slides

    $ cd slides/
    $ make

To tune the theme and colortheme, based on `slides/doc/`, please configure
`latex_theme` and `latex_colortheme` in Makefile.

## Resume

    $ cd resume/
    $ make

If no gravatar.jpg specified, a gravatar will be added automatically if the
email address is there. To disable this feature, do:

    $ GRAVATAR_OPTION=--no-gravatar make