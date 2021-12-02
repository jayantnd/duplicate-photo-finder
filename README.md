# duplicate-photo-finder
Find duplicate photos in Mac Photos App


I was having around 50k photos in my Mac with lots of Duplicates in it. Apple doesn't provide a tool to identity them. So wrote this small tool to delete those duplicate photos.

# How it works:
most(not all) of the duplicate photos will have same name with same size. so this tool will search all the photos with same name and size then create Album with current date (mm/dd/yy) and put them in Duplicates Photos folder.

Once it's added in the album you can go through the Album and delete them by pressing CMD+DELETE to delete permanently. (Though it’s very rare, album may contain photos which may not be duplicate. So be careful while deleting them)

# How to verify:
Copy a name of the photo from duplicate album and search, you will see more than one copy of same photo.
Also you can verify it by creating a duplicate photo, select recently duplicated photos, run this script


# Current Implementation
It uses a smart algorithm for faster processing. First it iterate all the selected Photos, then sort them using quick sort algorithm to have similar names together

then it iterate through the list again to group the similar named photos and place them in an Album in "Duplicate Photos" folder


# How to use:
open the script in script editor

open Photos app and select the photos you want to find duplicates in it.

then click on the run button.

# How to use in Terminal:
go to the folder in Terminal where you downloaded this script

open Photos app and select the photos you want to find duplicates in it.

run 'osascript duplicate-photo-finder.scpt'


#


Sit back and relax till the script complete its job.

It will take some time based on the count of phots selected in Photos App


#

Please give it a star if you find this tool useful :)
