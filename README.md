# Introduction

MFTParser was developed in C++ programming language to parse Microsoft Windows' MFT files on Linux. Use it as is. Testings have been done before this release. However, please feel free to reach out to me if any bugs are found.

# Version

0.2.1

# Usage

    Usage: mftparser [-h] [-a] [-j JOURNAL_FILE] [-r] [-w OUTPUT_FILE] [MFT_FILE]
    Version: 0.2.1
    Options:
    	-h,--help			        Show this help message
    	-a,--ads                    Show alternate data stream
    	-j,--journal JOURNAL_FILE	Parse journal file ($J)
    	-r,--resident			    Show resident data
    	-w,--write OUTPUTFILE		Output filename    

# Example

mftparser -w output.csv MFT

# Supported Output Format

L2TCSV (Unicode)

# Supported Operating Systems

- Ubuntu 14.04 x64 (tested)
- Ubuntu 16.04 x64 (tested)

It may work on other Linux distributions. However, testings are required to confirm them.

# SHA256

7921f1a06d2d7c356677a7c33b8d7c2077593697fca1ee0a7c6cf426dec24da1  mftparser
6bf2dd33f3a1fba3976fe45bccdedc8b9a445d1d10281d1aa6049a602e86130b  mftparser-0.2.1-Linux-x64.zip

# Dependency

libc++1

# Notes

- Currently, this tool only supports UTC.
- The date format is mm/dd/yyyy.
- The output file is unicode encoded.
- Unprintable characters in file names and resident data will be removed to prevent the L2TCSV format from being broken by them.
