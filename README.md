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
1. remove 'fcitx' which conficts with 'sogo'
```shell
sudo apt remove fcitx*
sudo apt autoremove
```
2. download from
http://pinyin.sogou.com/linux/?r=pinyin
3. install sogoupinyin
```shell
sudo dpkg -i sogoupinyin*.deb
sudo apt -f install
```
