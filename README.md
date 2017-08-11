# PacmanInitial
1. 新增一個java專案 
2. 官方抓 1.72， 利用現有marven project讀取之後
去 C:\Users\Josh\.m2\repository\uk\co\pacmanvghosts\pacman-main\1.0.5.2
找到pacman-main-1.0.5.2-sources.jar解壓縮，會出現
	data
	pacman
	META-INF
(此為source codes)
3. 官方抓解壓縮之後會產生
src/main/java
	entrants
	examples
	Main.java
4. 上述所有文件丟到新建專案的src資料夾

#需更改java檔
1.Game.java
	getGhostEdibleTime -> getGhostEdibleTime_new 		把 if(po)的檢查拿掉
	getGhostLairTime -> getGhostLairTime_new     		同上 
	getGhostCurrentNodeIndex - getGhostCurrentNodeIndex_new 同上
	isPillStillAvailable -> isPillStillAvailable_new
	isPowerPillStillAvailable -> isPowerPillStillAvailable_new
2.MyPacMan.java
 新增
import pacman.game.Constants;
import java.util.ArrayList;
import java.util.Random;
import java.io.*;
