#level12

##Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

##Solution
mktemp -d ;;make temporary file
ls
cp data.txt "tempdir";;copy file to temporary directory
cd "tempdir"
ls
mv data.txt data.hex;;change it to hex format
xxd -r data.hex data.bin;;change it to binary
ls
file data.bin ;; check the format
;; if the compressed data is in gzip 
;; we change the format of data.bin to data1.gz then decompress it by gzip -d data.gz
;; if in bzip2 we change it to .bz and decompress it by bzip2 -d filename
;; if it is in tar then we change it to .tar and decompress by tar -xf filename.tar we continue this process until Ascii text is get and the read the ASCII text file 
rm -rf "tempdir" to cleanup