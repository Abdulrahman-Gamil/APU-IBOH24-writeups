# APU-IBOH24 Write-ups

## Domain Expansion OSINT Challenge

### Challenge Description
![Challenge Description](https://github.com/user-attachments/assets/eeca2dd5-b731-4c7f-9cb2-7bbdbc152cc0)

### Provided Image
![Provided Image](https://github.com/user-attachments/assets/f775711b-e9ce-4a20-b894-e7335a2c5043)

### Analysis

The name of the train visible in the image is "Yamabiko." By conducting a quick search for "Yamabiko Line," we can confirm the train's name and also obtain a map of the stations on that line:

![Yamabiko Line Map](https://github.com/user-attachments/assets/5fdd940d-dac6-4fc9-9345-9661b4c1acc8)
![image](https://github.com/user-attachments/assets/208c9104-3a7e-45c0-971e-953191b4e587)


Next, we need to translate the Japanese text in the image to identify the name of the station:

![Station Name Translation](https://github.com/user-attachments/assets/ea47c90d-a7ab-46b5-86fb-0eea67679ba5)

The name of the station is **Shin-Hanamaki**, which is the first station on the route. 

### Determining the Second Station
To identify the second station, we notice the timestamps in the image: **Shin-Hanamaki at 11:47** and the next station at **12:36**. Although the name of the second station is not clear due to the blurriness of the image, we can refer to the train line map. 

From the map, we can see that the station adjacent to **Shin-Hanamaki** is **Kitakami**.


### the flag for this challenge is: `IBOH24{Kitakami_Station}`