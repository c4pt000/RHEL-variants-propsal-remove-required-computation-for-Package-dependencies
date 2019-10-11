# RHEL-variants-propsal-remove-required-computation-for-Package-dependencies
RHEL-variants-propsal-remove-required-computation-for-Package-dependencies

  &npsp;&npsp;&nbsp;yum or apt-get package manager attempts to figure out a group of package dependencies from an intertangled 
set of packages based on requirements or conflicts based per package, to install a particular package, a package 
might require several or more "dependent packages" in order for that set of package(s) to install for required 
libraries, headers, and other functions.
     &npsp;&npsp;&nbsp;yum or apt-get use processing resources on the computer's side to determine what dependencies are 
required to fetch and download in order to install, which can be sets of packages consisting of different quantities. 
     &npsp;&npsp;&nbsp;if different package configurations have hashed functions as a unique string in an algorithmic format md5 could be used to represent an entire set of packages as a predetermined list represented as an md5 string
the package manager could skip over trying to predetermine which dependent packages are required for different
types of package installations and just move directly to fetching and installing the required packages, 
as part of rpmdb(apt-cache) possibly or another downloadable data set type
    &npsp;&npsp;&nbsp; it would require a dry run of every known package based per operating system which uses computing resources to predetermine a set of packages (within that particular type of package manager) which are required as dependincies 
as part of the installation process per .
    &npsp;&npsp;&nbsp;hashing the current installed package list as a unique string md5 (or other variants then between the computer's side of installed packages checked against the server's side of available prehashed string, the matching strings would allow the package manager to just jump ahead to fetch(download) and install the required package configuration requests
   &npsp;&npsp;&nbsp;model to build unique strings based on installed packages compared to dependent package requirements for string generation systems that require downloading packages from client to server could assemble unique values of package requirement types
based on a pass (1) of a successful installation install (from rpmdb's current installed packages as a unique string)
    &npsp;&npsp;&nbsp;a pattern of packages that checkout and install successfully without an error generate a unique string based on that successful package configuration installation and are appended to the server side's database of precomputed package possibilites
