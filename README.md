# ubuntu-setup-auto-by-command-line

        Follow these steps in order to install OpenVPN 3 Client on Linux for Debian and Ubuntu:

            Open the Terminal by pressing ctrl + alt + T

            Type the following command into the Terminal: sudo apt install apt-transport-https. This is done to ensure that your apt supports the https transport. Enter the root password as prompted

            Type the following command into the Terminal: sudo wget https://swupdate.openvpn.net/repos/openvpn-repo-pkg-key.pub. This will install the OpenVPN repository key used by the OpenVPN 3 Linux packages

            Type the following command into the Terminal: sudo apt-key add openvpn-repo-pkg-key.pub

            Type the following command into the Terminal: sudo wget -O /etc/apt/sources.list.d/openvpn3.list https://swupdate.openvpn.net/community/openvpn3/repos/openvpn3-$DISTRO.list. This will install the proper repository. Replace $DISTRO with the release name depending on your Debian/Ubuntu distribution (the table of release names for each distribution can be found below). In this case, focal is chosen since Ubuntu 20.04 is used

            Type the following command into the Terminal: sudo apt update

            Type the following command into the Terminal: sudo apt install openvpn3. This will finally install the OpenVPN 3 package
