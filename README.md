argparse-exam
=============


$ java Checksum -h
usage: Checksum [-h] [-t {SHA-256,SHA-512,SHA1}] [file [file ...]]
 
Calculate checksum of given files.
 
positional arguments:
  file                   File to calculate checksum
 
optional arguments:
  -h, --help             show this help message and exit
  -t {SHA-256,SHA-512,SHA1}, --type {SHA-256,SHA-512,SHA1}
Specify hash function to use (default: SHA-256)

$ java Checksum file1.cc file1.h
6bd85bf4b936bc8870c70bea04cd12d4fe3745934f511e6e188d718d32154a79  file1.cc
839ef370cbd54f62985bac7b974cc575eaaa24a8edd6ae7787cfc71829ceda40  file1.h


$ java Checksum -t SHA1 file1.cc
20bada64dde97b98faaba09ebbfdb70af71476f1  Checksum.class
