# esp32camToSD
esp32-cam module take image to sd, enter deep sleep and wake up again

Thanks to Rui Santos for his work[1]. 
Pinout didn't change. 
Unsolder LED which is also connected to SD-Pin Data1
It's modified to take a picture save it to SD-Card, enter deep sleep for fixed time afterwards.
Also added SD_MMC.end(); to make sure SD is unmounted and filesystem doesn't get corrupted.

[1] https://randomnerdtutorials.com/esp32-cam-take-photo-save-microsd-card
