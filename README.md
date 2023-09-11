# cub3d_tester
A simple tester for cub3d

| ⚠️ This tester is for Linux only ⚠️ |
| --- |

| ⚠️ You should add or update map files to accommodate how you handle spaces for the map! ⚠️ |
| --- |


## Quick start
- Put all files inside the root of your project.
- Run `bash tester.sh`

During testing, a window will open for each map (for invalid maps this *may* not be the case). You can interact with that map and then close the window (or press ESC) to continue.

🚨 There's a test you should do with maps like `./maps/valid/triangle.cub` which consists in walking straight into a corner. The raycast may trigger a segfault depending on your implementation because you may walk trought the corner, making the raycast unable to calculate the distance to the next wall.

```
[ ][1][ ]<- the raycast may go forever
[1][N][1]
[ ][1][ ]
```


## Adding more tests
1. Put the files inside the **maps/valid/** or **maps/invalid/** folders and add them to the appropriate list inside `tester.sh`
2. Put the textures for your new map files inside the **textures/** folder (unless you're testing for missing texture files)



## Things to take away
- This tester may not cover all tests!
- Trust no one. It is your responsibility to make sure everything works correctly.
- Explore the script and try to adapt it to other things. Testing is a highly valuable skill that should not be overlooked! Seize the opportunity to learn it!
