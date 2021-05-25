# project
* Seperate the multi-page tif into single pages (IMAGEMAGICK)

Go to the goal folder:  
(Scene 0: the number from 0) 
```
Convert -scene 0 abc.tif abc_%d.tif
```
OR
```
convert A.tif -set filename:f "%[t]_%[fx:t+1]" +adjoin "%[filename:f].tif”
```
Out:A_1.tif , A_2.tif, A_3.tif, A_4.tif, A_5.tif, A_6.tif, A_7.tif, A_8.tif, A_9.tif, A_10.tif
* Generate point_cloud and create ply file
* Visualize it by using Open3D
