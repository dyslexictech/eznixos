Welcome to eznixOS

The eznixOS is a respin of Debian GNU/Linux, currently based on the Debian 10 Buster release. The Debian live-build tool is used to build the ISO and I have included a folder located under /usr/share/eznixOS109/eznix109 containing all the necessary build files and build script used to create the respin. I include all the files with the aim to help educate those willing to learn how to build your own live-build created Debian respins.

This respin was built by my bldeznix109 script but can also be built identically by following the prepare-howto.txt and bldeznix109-howto.txt files. The build process has been completely automated as long as you do not need to make any adjustments. The bldeznix109 will build a complete respin of Debian Buster with all of the eznixOS customizations. If you want to utilize the script to produce your own respin, you will need to edit various parts of the script. The script is documented and should be easy enough to rework into something personal for you.

The ISO contains all the eznixOS build related files inside the /usr/share/eznixOS109/eznix109 folder. Any changes to the files or the folder names must be represented in the bldeznix109 script. The script relies on certain folder names and files to operate correctly. Read the comments in the bldeznix109 script and the prepare-howto.txt and bldeznix109-howto.txt files for guidance. The /eznix109 folder must reside in the same directory as the bldeznix109 script. Anything can be changed to suit your needs, but the changes must be identical in both the script and the folder structure around it.

The ezadmin tool is a small script with a menu driven interface that performs a few basic functions. The basic functions of the ezadmin tool are to add the first user to the sudo group. Many users find sudo a convenient method to temporarily gain root privileges to perform administrative tasks. The ezadmin tool can also optimize the sources.list file, adding the contrib and non-free sections to the repositories and switching the mirrors to Debian's DNS based redirection servers for automatically picking the closest mirrors. Please take a look at the ezadmin-howtow.txt on the Desktop of eznixOS.

#################################################
#                                               #
# -------------------                           #
#  EZ Admin Menu:                               #
# -------------------                           #
#                                               #
#  (a) Add Myself to Sudo Group                 #
#       (Logout & Login to take effect)         #
#  (b) Optimize Sources	& Update Repos          #
#  (c) Update Youtube-dl to latest version      #
#  (d) Enable systemd-resolved service          #
#  (e) Install or upgrade Firefox Latest        #
#  (f) Install newest kernel from backports     #
#       (Reboot Required)                       #
#                                               #
#  (x) Exit                                     #
#                                               #
# Please enter your choice:                     #
#                                               #
#################################################

You can run the ezadmin script as root to perform its functions. Use "su -l" to root in a terminal and issue the command: "ezadmin" to execute the script. Read the documentation for the ezadmin script BEFORE using it. The functions are serious and the changes are not easy to reverse once done. Have fun.


# readme.txt -- Revision: 109r1 -- by eznix (https://sourceforge.net/projects/eznixos/)
# (GNU/General Public License version 3.0)
