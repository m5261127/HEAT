# HEAT

HEAT is a software package for thermal cameras;\
*Hayabusa2&Hera Exploration Assistant for TIR&TIRI.*

This software can do below things.

1. To display TIR images and thermal models 
1. To calibrate TIR interactively
1. To convert TIR DN image to temperature one.
1. To use TIR database (ground test & obserbation)

***Hera/TIRI data will be supported in the future.***




![HEAT_functions](https://user-images.githubusercontent.com/120307289/207242713-ccd678da-c9e2-49db-b355-d5759525cd2a.png)

# ScrennShots
#### Database and Visualization
![HEAT_SS_all](https://user-images.githubusercontent.com/120307289/207242524-04d970ad-c9de-491d-b1b2-125c2d818449.png)
#### Calibration
![HEAT_SS_cal](https://user-images.githubusercontent.com/120307289/207242527-45f90848-bf7b-4212-869f-71e5637efae2.png)

# Requirement
#### Windows and Linux will be supported in the next update.
### MacOS
- OS
  - MacOS
    - Bigsur, Catalina, Mojave
- [Xcode](https://developer.apple.com/jp/xcode/) graeter than 11
  - C++ 11
- [Qt](https://www.qt.io) 5.14
- [Homebrew](https://brew.sh/index)
- [cfitsio](https://heasarc.gsfc.nasa.gov/fitsio/) 2.6
- [ccfits](https://heasarc.gsfc.nasa.gov/fitsio/ccfits/) 4.1
- [Spice tool kit](https://naif.jpl.nasa.gov/naif/toolkit.html)
- [MySQL](https://www.mysql.com/) 5.7



# Installation

#### XCode
Install from App Store.\
C++ is installed at the same time.

#### Qt 5.14
Install from [official web site](https://www.qt.io/download-qt-installer?hsCtaTracking=99d9dd4f-5681-48d2-b096-470725510d34%7C074ddad0-fdef-4e53-8aa8-5e8a876d6ab4) and launch the online installer.\
Select Qt 5.14 and QtCreator in the installer.

#### Homebrew
Read [official website](https://brew.sh/index) carefully and install it.

#### Other

```bash
brew install cfitsio
brew install ccfits
brew install cspice
brew install mysql@5.7
```

The PRO file is the file that makes up the project.\
After you install the necessary modules, you need to set the path.\
Please refer to HEAT.pro for more information.

# Usage
#### Conversion
![HEAT_3](https://user-images.githubusercontent.com/120307289/207309416-ced044d7-c2ef-493e-af02-96b1699c2a67.gif)

#### Visualization of the Ryugu data
![HEAT](https://user-images.githubusercontent.com/120307289/207255328-e329bc87-37fb-4c2d-bb70-a66a0d7e5af8.gif)
#### [Data](https://data.darts.isas.jaxa.jp/pub/pds4/data/hyb2/hyb2_tir/) published on Jaxa can be used in HEAT.


# Note

* Qt cannot be installed without installing XCode in MacOS.
* To use the database and calibration functions, a separate database file is required. Please contact us if you need one.
* Other referenced files must be included in the application.
![HEAT_2](https://user-images.githubusercontent.com/120307289/207267548-eee94df1-8d87-47b9-9aa0-724e6e46f415.gif)
* If you get the message "QMYSQL driver not loaded", you need to read [official web page](https://doc.qt.io/qt-6/sql-driver.html) and configure the driver. However, if you do not use the database function, you do not need to configure it.

# Contacts
* E-mail:heat-develop@u-aizu.ac.jp

# License
(c) 2022 [The University of Aizu](https://u-aizu.ac.jp/)\
This software is released under the [GNU General Public License](https://en.wikipedia.org/wiki/GNU_General_Public_License).

