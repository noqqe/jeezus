# jeezus...

jeezus is an experimental smtp proxy that I wrote to be able to do serverside bayesian
spam filtering. In this case using `bogofilter`.

![](https://github.com/noqqe/jeezus/raw/master/christ.jpg)

### Usage

Usage is easy.

    ./jeezus --listen 127.0.0.1:12000 --deliver 127.0.0.1:25 --pipe-command '/usr/local/bin/bogofilter -u -e -R'

or using short flags.

    ./jeezus -l localhost:4451 -d localhost:25 -p "/usr/local/bin/bogofilter -u -e -p -R"

In use with `bogofilter` it is necessary that the called command is
echoing the original mail (and added X-Headers with spam scores)

### Embedding example

todo..

### Requirements

Just install `inbox.py` using pip and python2.7

    pip install inbox.py
