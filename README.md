● Introduction

MFTParser was developed in C++ programming language to parse Microsoft Windows' MFT files ($MFT) on Linux. This is an initial release. Use it as is. Testings have been done before this release. However, please feel free to reach out to me if any bugs are found.

● Usage

Usage: mftparser [-h] [-j JOURNAL_FILE] [-w OUTPUT_FILE] [MFT_FILE]
Version: 0.1.0
Options:
	-h,--help			Show this help message
	-j,--journal JOURNAL_FILE	Parse journal file ($J)
	-w,--write OUTPUTFILE		Output filename

● Example

mftparser -w output.csv MFT

● Supported Output Format

L2TCSV (UTF-8)

● Supported Operating Systems

Ubuntu 14.04 x64 (tested)
Ubuntu 16.04 x64 (tested)

It may work on other Linux distributions. However, testings are required to confirm it.

● SHA256

6c171511c0fcadca038254d225fda9fe7d6f637935afb0a0f43c7db289ddb242  mftparser
15cbddeba833b50ab14fea03050263467968f9d8aef572e6bff2894af779b2e2  mftparser-0.1.0-Linux-x64.zip

● Dependency

libc++1

● Notes

- Currently, this tool only supports UTC.
- The date format is yyyy-mm-dd.
- The output file is UTF-8 encoded. 
    
