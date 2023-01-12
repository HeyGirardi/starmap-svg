##### Requirements 
###### Python > 3.2
```pwsh
pip install svgwrite
```
##### Usage
```pwsh
python starmap.py
```
| arguments | description                               |
| :-------- | :---------------------------------------- |
| -h        | show help message and exit                |
| -cons     | show constellations True/False            |
| -coords   | coordinates in format nortern,eastern     |
| -date     | date in format day.month.year             |
| -guides   | draw guides True/False                    |
| -height   | height in mm                              |
| -info     | text displayed above coordinates          |
| -magn     | magnitude limit 0.1-12.0                  |
| -output   | output file                               |
| -summer   | if it is summertime on the specified date |
| -time     | time in format hour.minute.second         |
| -utc      | utc offset of location -12 to +12         |
| -width    | width in mm                               |
##### Example 1
```pwsh
python starmap.py -coord 60.186,24.959 -time 12.00.00 -date 01.01.2000 -utc +2 -constellation True
```
![image](https://github.com/skeletor-git/starmap-svg/blob/master/example/starmap.png)
##### Example 2
```pwsh
python starmap.py -coord 35.684,139.728 -time 20.00.00 -date 15.07.2018 -utc +9 -info TOKYO -guides True -magn 10.0 -width 150 -height 220
```
![image](https://github.com/skeletor-git/starmap-svg/blob/master/example/starmap2.png)
#### Info
Stars data: "Yale Bright Star Catalog ver5"
http://tdc-www.harvard.edu/catalogs/bsc5.html
