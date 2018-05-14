# cheatsheets

## cheat sheets websites
https://devhints.io/

## Matplotlib tutorial
https://www.datacamp.com/community/tutorials/matplotlib-tutorial-python

## Unix one line
### rsync 
```shell
rsync -avzuc ./src /dest
```
### install package via bundle
```shell
chmod a+x xxx.bundle
sudo ./xxx.bundle
```
## Unix softwares
### sogou pinyin
```shell
sudo apt install libopencc1 fcitx-libs fcitx-libs-qt fonts-droid-fallback  
sudo dpkg -i sogoupinyin_xxxx.deb  
```
deb can be downloaded here https://pinyin.sogou.com/linux/?r=pinyin.
If error occurs, removing installed 'sogou' (via command below) and resintalling 'fcitx' and 'sogou' (run the commands above ageain) should solve the problem.
```shell
sudo apt remove sogoupinyin  
```
### latex
```shell
sudo apt-get install texlive-full  
sudo apt-get install texmaker
```
