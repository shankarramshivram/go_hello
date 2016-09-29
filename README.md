#My Motivation behind learning GoLang

 - As the FAQ of GoLang tells --  .. i wanted something which combined ease of programming , efficient compilation, efficient execution & fast.


# Installing Go
1. Download go stable from their downloads release page.
2. Untar and mv to /usr/local
3. Set GoLang env variables in the bashrc. (By default Go assumes that the go installation location will be in  /usr/local if not then wer have to export GOROOT also)
..* export GOPATH=<workspace>
..* export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin

# Some Basic Notes regarding workspaces .. how things are arranged etc.etc....

What is  a workspace ?
Its a directory hierarchy with 3 directories at its root :-
1. src ( go source files)
2. pkg ( package objects)
3. bin (executables)

go tool -- builds packages from source files in src and installs the resulting binaries in pkg and bin directories

#Setting up Atom with GO --
1. In Ubuntu -- you have to start atom from commandline so that bashrc is sourced and GOPATH is Setting
2. Next following the instructions from the  3 links below  helped setup my atom environment  
..* https://rominirani.com/setup-go-development-environment-with-atom-editor-a87a12366fcf#.qi484xegk
..* https://docs.google.com/document/d/1C3lg2el_-uKvm64JNwUNJzgnu0UfrH_PmWyBetB73jw/edit
..* https://www.youtube.com/watch?v=3RS7LyBt8aA
