# grf
multi-threads gen random files

### Download
download prebuild binary  
https://github.com/vager/grf/releases  
or build from source
```
git clone https://github.com/cchare/grf.git
cd grf
go build
```

### Usage
##### help page
```
./grf -h
Usage of ./grf:
  -n uint
    	number of files (default 1)
  -o string
    	output dir (default ".")
  -p string
    	filename prefix (default "vager")
  -s string
    	size(K,M,G,T) of file (default "1M")
  -t int
    	threads (default 8)
  -v	show version
```

##### Generate 16 random files with size 2.2M to current dir
```
./grf -n 16 -s 2.2M
```

##### Use 16 theads generate 16 random files to outdir/
```
mkdir outdir
./grf -t 16 -n 16 -o outdir
```
