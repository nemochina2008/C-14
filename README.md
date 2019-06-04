# C-14

## C++14 standard requested but CXX14 is not defined

Mm <- file.path(Sys.getenv("HOME"), ".R", ifelse(.Platform$OS.type == "windows", "Makevars.win", "Makevars"))
file.edit(Mm)

## adding below to Mm files and save... 

CXX14=$(BINPREF)g++ -O2 -march=native -mtune=native
CXX14FLAGS=-O3 -march=native -mtune=native
CXX11FLAGS=-O3 -march=native -mtune=native
