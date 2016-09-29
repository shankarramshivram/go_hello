#My Motivation behind learning GoLang

 - As the FAQ of GoLang tells --  .. i wanted something which combined ease of programming , efficient compilation, efficient execution & fast.


# Installing Go
1. Download go stable from their downloads release page.
2. Untar and mv to /usr/local
3. Set GoLang env variables in the bashrc. (By default Go assumes that the go installation location will be in  /usr/local if not then wer have to export GOROOT also)
  * export GOPATH=<workspace>
  * export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin

# Some Basic Notes regarding workspaces .. how things are arranged etc.etc....

What is  a workspace ?
Its a directory hierarchy with 3 directories at its root :-
* src ( go source files)
* pkg ( package objects)
* bin (executables)

go tool -- builds packages from source files in src and installs the resulting binaries in pkg and bin directories

#Setting up Atom with GO --
1. In Ubuntu -- you have to start atom from commandline so that bashrc is sourced and GOPATH is Setting
2. Next following the instructions from the  3 links below  helped setup my atom environment  
  * [Link 1 - Medium ] (https://rominirani.com/setup-go-development-environment-with-atom-editor-a87a12366fcf#.qi484xegk)
  * [Link 2 - Google Doc] (https://docs.google.com/document/d/1C3lg2el_-uKvm64JNwUNJzgnu0UfrH_PmWyBetB73jw/edit)
  * [Youtube Video] (https://www.youtube.com/watch?v=3RS7LyBt8aA)

## Folder 002 - GO Basics - Source : [Free Book] (https://astaxie.gitbooks.io/build-web-application-with-golang/content/en/02.2.html)

### Variables :
  * Single Variable - var varname type
  * Multiple Variables - var varname1 varname2 varname3 type
  * Variable with 1 value - var varname type = value
  * Multiple Variables with values - var varname1, varname2, varname3 type = value1, value2, value3
  * Another way to declare variables (only works inside functions ) is
    * varname1, varname2, varname3 __:=__ value1, value2, value3
  * Variables declared but not used will give compilation errors.

### Constants :
  * Values that are determined during compile time and cannot be changed during
  run time.

### Boolean
  * Same as other lang -- takes  only 2 values --  True / False.

### Numeric Types
  * int, uint, byte, complex64 etc etc..

### Strings
  * Represented by "" , uses UTF-8 character set.
  * Cannot directly change characters in astring. Instead we convert the String
  to array of bytes -> then change the character -> then change to string again.
  * Can combine two strings using the + operator

### Defining variables,Constants, import packages by group
  * Sample :
    * import (
      "fmt"
      "os"
    )
    * const (
      i = 100
      pi = 3.1415
      prefix = "_Shank_"
    )
    * var (

      )

      )
### iota -- This keyword is for enum, starts at 0 and increases by 1

### Array
  * var arr [n]type
  * a := [...]int{1, 2, 3} (... -- go will calculate the length )
  * Multidimensional Arrays
    * sampleArray := [2][4]int{{1, 2, 3, 4}, {6, 7, 8, 9}}
  * When arrays are passed as arguments to a function , the function gets a copy
  and not the reference. If reference is needed then use slice

### Slice : - Similar to the function of a dynamic array.
  * without ... in [] we declare slice.

### MAP -  Behaves like python dictionary
### make, new
  * make -- memory allocation for built in models --- map , slice .

### Control Statements
  * if , for , switch
### functions
  * func <funcname> (argument1, argument2 ...) (return1...return n) {}

### Functions as values and Types
... MTBW
### Defer, Panic, Recover
... MTBW

### Pointers come back to my life  :P
... MTBW

## Go Rules
  * No public or private keyword .Any variable/function/Constants that begins with capital letter means it will be exported.

## Useful Free links i am following

  * [Web application building with golang](https://astaxie.gitbooks.io/build-web-application-with-golang/content/en/02.4.html)
