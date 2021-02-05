![alt text][logo]

Avnet Board Definition Files (BDF)
==================================

Official repository of all Avnet Board Defintion Files which can be used with Xilinx Vivado HLx tools.

This repository is intended to provide publicly accessible, revision control for all current Avnet Board Definition Files for Xilinx Vivado HLx tools.

Disclaimer:

Avnet, Inc. makes no warranty for the use of these design files.  The files are provided  "As Is". Avnet, Inc assumes no responsibility for any errors, which may appear in these files, nor does it make a commitment to update the information contained herein. Avnet, Inc specifically disclaims any implied warranties of fitness for a particular purpose.


Current Tools Version:
----------------------

* **Version Agnosti**c [Vivado 2018.3+]


Installing the Avnet Board Definition Files Under Windows
---------------------------------------------------------

Please download and copy the desired Board Definition Files from this [BDF] repository to the following folder of the Vivado 2018.3 install directory on your Windows development PC:

*__<install_location>\Vivado\2018.3\data\boards\board_files__*

Once the files are copied to the appropriate Vivado install sub-folder, launch Vivado Design Suite 2018.3 to be able to access the Avnet boards through the new project creation wizard or use one of the scripted project builds from the Avnet [hdl] repository.


Installing the Avnet Board Definition Files Under Ubuntu
--------------------------------------------------------

Please download and copy the desired Board Definition Files from this [BDF] repository to the following folder on your Ubuntu development PC:

*__/tools/Xilinx/Vivado/2018.3/data/boards/board_files__*

Once the files are copied to the appropriate Vivado install sub-folder, launch Vivado Design Suite 2018.3 to be able to access the Avnet boards through the new project creation wizard or use one of the scripted project builds from the Avnet [hdl] repository.


Detailed Instructions for Installing Files Under Ubuntu without using Git
-------------------------------------------------------------------------

1. In your browser, load up the Avnet [BDF] repository.

2. Select *__Clone or download__* at the top of the page and then select the *__Download ZIP__* to download the Board Definition File *__bdf-master.zip__* archive to a temporary download folder onto your local Ubuntu development PC.

![alt text][download_zip]

3. Under Ubuntu, we need to make sure that read and write permissions for Vivado tools folder are set as expected to allow you to install the Board Definition Files in the correct location.  Open a terminal and run the following commands (Note: This is assuming you followed the latest Avnet [VM Installation Guide] or have installed Vivado on your native Ubuntu development PC using the default install location):

`$ cd /tools/Xilinx/Vivado/[version]/data/boards/`

`$ sudo chown training -R board_files`

`$ sudo chgrp training -R board_files`

4. Now that we have changed the permissions of the Vivado board_files folder, we now need to unzip the contents of the bdf-master.zip archive from your download folder into the home directory *__~/__* for the current user.

![alt text][locate_zip]

5. After copying the *__bdf-master.zip__* to the home directory we now want to unzip the folder and then copy them into the *__/tools/Xilinx/Vivado/2018.3/data/boards/board_files__* directory. Open a terminal and run the following commands:

`$ cd ~`

`$ unzip bdf-master.zip`

`$ cp -a ./bdf-master/. /tools/Xilinx/Vivado/[version]/data/boards/board_files`

6. Feel free to delete any BDF files located in your home directory or temporary download locations for the *__bdf-master.zip__* archive.  Now that all board definition files are copied to the correct vivado *__board_files__* directory you are ready to start development work using built-in tools support for Avnet boards.  If you are unsure of where to start, please check out the latest Avnet [Technical Training Courses] for these boards which will provide you a great deal of information on how to best utilize the Xilinx tools and maximize the utility of your Avnet board as a development platform for your next system design.


Where can I get support?
------------------------

For design support please contact your local Avnet FAE or visit one of our support forums:

* For design-in product support for ZedBoard, MicroZed, PicoZed, MiniZed, UltraZed, or Ultra96 please access our Element14 community support forums at [Element14 Zed Community Support Forums].

* Please access the [Element14 Zed Community] for all other engineering boards, products, and tools support inquiries.


I am an engineer, I found a bug and I want to contribute the fix back into this repo, how can I submit changes?
---------------------------------------------------------------------------------------------------------------

* First of all, thank you for contributing!

* Please contact the support forum for the Avnet board you are using.


I am an engineer at Avnet, how can I submit code changes?
---------------------------------------------------------

* Please contact the Avnet Products Group for further details.

[Vivado]:https://www.xilinx.com/products/design-tools/vivado.html
[Element14 Zed Community]:http://avnet.me/zed-community
[Element14 Zed Community Support Forums]:http://avnet.me/zed-forums
[VM Installation Guide]:http://avnet.me/vm_install
[Technical Training Courses]:http://avnet.me/TTC
[BDF]:https://github.com/Avnet/bdf
[hdl]:https://github.com/Avnet/hdl
[download_zip]:https://github.com/Avnet/bdf/blob/master/download_zip.png "Download Zip"
[locate_zip]:https://github.com/Avnet/bdf/blob/master/locate_zip.png "Locate Zip"
[logo]:https://github.com/Avnet/legal/blob/master/avnet_logo.png "Avnet"
