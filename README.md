# PVSio-Projects

Repository for projects on PVSio-web (http://www.pvsioweb.org). PVSio-web is a graphical tool for prototyping and analyzing user interface software based on formal models. To test the projects, it is necessary to install the PVS language and preferably install the PVSio-web server locally.

## Installation

To install PVSio-web, first you need to install PVS and NodeJS, and then clone the PVSio-web github repository (https://github.com/pvsioweb/pvsio-web).

**Note:** The tool is only available for Linux and MacOs.

#### Step 1: Install PVS and add PVS executables to your PATH
PVS is required to run PVSio-web. The tool can be downloaded at http://pvs.csl.sri.com/downloads.html Installation instructions can be found on the website.

Once PVS is installed, you must add the PVS executable files to your PATH: *pvs*, *pvsio* and *profit*. A simple way to do this is to create symbolic links to these files and place the symbolic links in /usr/bin. For example, if PVS is installed in /opt/PVS/pvs, the following commands executed in a Terminal window create the necessary symbolic links:

    sudo ln -s /opt/PVS/pvs /usr/bin/pvs
    sudo ln -s /opt/PVS/pvsio /usr/bin/pvsio
    sudo ln -s /opt/PVS/proveit /usr/bin/proveit

Please note that the ln command requires a full path.

**Note:** There is also a plugin for Visual Studio Code. You can learn more here https://github.com/nasa/vscode-pvs

#### Step 2: Install NodeJS
NodeJS is also required to run PVSio-web. Download and install NodeJS at http://nodejs.org
Installation instructions are on the website.

#### Step 3: Clone the PVSio-web repository
Create a directory where you would like to install PVSio-web on your local computer. Open a Terminal window in the created directory, and use 'git' to clone the PVSio-web repository:

    git clone https://github.com/thehogfather/pvsio-web.git
    cd pvsio-web
    npm install

PVSio-web is now installed on your local computer!

#### Step 4: Running pvsio-web

To run pvsio-web, open a Terminal window in the pvsio-web directory and use the following command (leave the Terminal window open):

    ./start.sh

The browser should open automatically, otherwise, open the browser of your choice and enter the following address in the address bar:

    http://localhost:8082/

#### Updating pvsio-web

To update pvsio-web to the latest version, in a Terminal window, run the following command in the pvsio-web directory:

    git pull

---

## Opening projects
