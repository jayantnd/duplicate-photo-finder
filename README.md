# duplicate-photo-finder
Find duplicate photos in Mac Photos App


I was having around 50k photos in my Mac with lots of Duplicates in it. Apple doesn't provide a tool to identity them. So wrote this small tool to delete those duplicate photos.

# How it works:
most(not all) of the duplicate photos will have same name. so this toll with search all the photos with same name and create Album with same named photos and put them is a separate folder.
Once its grouped and placed in a album you can go through the Ambums and delete them. (Album may contain photos which may not be duplicate. SO be careful while deleting them)

# Current Implement
First it iterate all the selected Photos, them sort them using quick sort algorithm to have similar names together
then it itereate throught the list again to group the similar named photos and place them in an Album in "Duplicate Photos" folder

# Future improvements: 
This can be improved by using a dictionary to group the same named photos to avoid one iteration.
Any PR will be most welcome for improvement

# How to use:
open the script in script editor
open Photos app and select the photos you want to find duplicates in it.
then click on the run button.

# How to use in Terminal:
go to the folder in Terminal where you downloaded this script
open Photos app and select the photos you want to find duplicates in it.
run osascript duplicate-photo-finder.scpt

Sit back and relax till the script complete its job.
It will take some time based on the count of phots seleceted in Photos App
