# search-and-replace-renamer
<p align="center">
  <img width="49%" alt="Empty gui" src="https://github.com/user-attachments/assets/eac8f9fc-c84a-4857-95a1-fc6d5cfbef7e" />
  <img width="49%" alt="Gui with files" src="https://github.com/user-attachments/assets/d2e88924-69f4-4931-895b-5a5d5c0498cf" />
</p>

### 99% of work belongs to [dubrowgn](https://github.com/dubrowgn). I just made some minor changes.
So, basically original Renamer is a lightweight, mass file renaming utility based on the Qt framework. It's designed to be very simple yet robust with it's drag-n-drop interface and use of regular expressions.

**Main Features**
* Cross-Platform
* Drag-n-Drop interface
* Regex search and replace
* Literal search and replace
* Renames files and folders

**My Changes**
* Gui theme changed from light to dark
* Unchecked `Use Regex` by default
* Fixed icon.ico
* Less program size
* Some gui changes for better experience.

## How to use
1. [Download](https://github.com/br0d96a/search-and-replace-renamer/releases/download/v1.0/renamer.exe) and run.
2. Drag-n-drop files/folders in gui.
3. Fill the `Search` and `Replace` fields.
4. Press `Search and Replace` button.

Some tips. 
* You can select one or many items with mouse, using `CTRL` as well.
* Copy name of selected item with `CTRL+C`.
* Use `Delete` key to delete selected items ***from gui list***.

### Notes
*By me: I have only Windows build, for others you must do it yourself or go to original [renamer](https://github.com/dubrowgn/renamer) releases.*

*By dubrowgn: The linux build of Renamer now requires Qt 5.6 or greater be installed. On Debian/Mint/Ubuntu distros, you can install the `libqt5gui5` package via `apt-get`.*

## How i build

**Qt 5.15.2 (MinGW-w64 GCC 8.1.0 64-bit)  
Perl 5.32.0 x64  
Python 2.7.18**  

```
configure.bat -opensource -confirm-license -release -static -optimize-size -no-ltcg -no-opengl -gc-binaries -nomake examples -nomake tests -nomake tools -skip qt3d -skip qtactiveqt -skip qtandroidextras -skip qtcharts -skip qtconnectivity -skip qtdatavis3d -skip qtdeclarative -skip qtdoc -skip qtgamepad -skip qtgraphicaleffects -skip qtlocation -skip qtlottie -skip qtmacextras -skip qtmultimedia -skip qtnetworkauth -skip qtpurchasing -skip qtquick3d -skip qtquickcontrols -skip qtquickcontrols2 -skip qtquicktimeline -skip qtremoteobjects -skip qtscript -skip qtscxml -skip qtsensors -skip qtserialbus -skip qtserialport -skip qtspeech -skip qtsvg -skip qttools -skip qttranslations -skip qtvirtualkeyboard -skip qtwayland -skip qtwebchannel -skip qtwebengine -skip qtwebglplugin -skip qtwebsockets -skip qtwebview -skip qtx11extras -skip qtxmlpatterns -prefix C:\QtBuild\static-5.15.2
```
