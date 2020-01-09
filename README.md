# Marginal-0verseas
邊緣人海聯樹莓派專案 - ELK

## 介紹
利用 ELK 抓取海聯機器上的日誌進行資料蒐集、分析、統計等，之後用 reapberry pi 進行視覺化的工作呈現圖表。

## 部署
### 安裝 Raspbian Buster Lite
1. 燒錄 image 至 microSD 卡中，插入樹莓派並接上電源開機
2. `sudo raspi-config` 打開 SSH 及其他自己想要的功能或設定後，`sudo shutdown -r now` 重啟樹莓派
3. `sudo apt update` 更新套件資訊
### 安裝 GUI 及瀏覽器（由 Raspberry pi 直接輸出至螢幕者需要）
#### Raspberry Pi Desktop (RPD) GUI
1. `sudo apt install --no-install-recommends xserver-xorg`
2. `sudo apt install --no-install-recommends xinit`
3. `sudo apt install raspberrypi-ui-mods` （如果不想裝正常版，可選精簡版 `sudo apt install --no-install-recommends raspberrypi-ui-mods lxsession`）

※此處步驟1、2是安裝GUI中必須要的，第三步開始可選擇自己喜歡的 GUI
#### 安裝瀏覽器
擇一喜歡或自己慣用的瀏覽器即可
##### Epiphany
`sudo apt install epiphany-browser`
##### Firefox
`sudo apt install firefox-esr`
##### Chromium
`sudo apt install chromium-browser`

## 成員
1. 陳荷文(真．組長)
2. 洪煥銘
3. 賴王bin

## 設備
名稱 | 數量 | 來源
---- | ---- | ----
Raspberry Pi 3 | 1 | 課堂借用
HDMI 線 | 1 | 煥銘買螢幕附的
螢幕 | 1 | 煥銘桌上的螢幕剛好有支援 HDMI 輸入

## 參考資料
* [在 raspbian buster lite 上安裝 Raspberry Pi Desktop (RPD) GUI](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=133691)
