# APU-IBOH24 Write-ups

## Positive Aura Stalker OSINT Challenge

### Challenge Description
![Challenge Description](https://github.com/user-attachments/assets/ebfaf7c1-5d56-4f80-a186-1ca5c16635f7)

### Provided Image
![Provided Image](https://github.com/user-attachments/assets/ed2d9231-5683-4f88-ba9e-d62c06113c16)

### Analysis

The first step is to identify the American boxer referenced in the provided image. By using Google Lens, we can analyze the object in the image and try to find a match:

![Google Lens Result](https://github.com/user-attachments/assets/2a559ea7-33fc-4f0b-8fc4-ee5a74e60aa6)

The object in our provided image matches with an object found on a website about **Muhammad Ali**, the famous boxer.

### Identifying the Boxer's House

Next, we search for Muhammad Ali’s house and uncover some details:

![Boxer's House Search](https://github.com/user-attachments/assets/adc915d4-4338-4036-bc5b-7e7d53ea8411)

One of the websites reveals that Muhammad Ali lived with his parents in **Louisville, Kentucky**.

### Narrowing Down the Location

In the provided image, we can see a house number: **1963**. Now that we know the house number and the hometown (Louisville, Kentucky), we perform further searches:

![House Number Search](https://github.com/user-attachments/assets/afe65a63-ec90-4f45-b414-6b09ec923148)

We find several houses with the number **1963**:
1. Norris Pi
2. Meadowcreek Dr
3. Richmond Dr
4. Douglass Blvd

Upon examining the provided image again, it looks like **Richmond Dr** matches part of the house shown. To confirm, we look at this house using Google Maps:

![Google Maps Analysis 1](https://github.com/user-attachments/assets/f740070c-e50b-4e9c-a280-0ac56d297130)
![Google Maps Analysis 2](https://github.com/user-attachments/assets/f9fcfc17-49e4-4a1e-ba98-bfee5dd0e3fd)

Using Google Maps, we can see the house is located between two streets: **Richmond Dr** and **Kenilworth Pl**.

### Final Confirmation

To finalize, we analyze the alley and the surroundings of the house:

![Alley Analysis 1](https://github.com/user-attachments/assets/018ff306-1af4-40d3-a3b9-b172a7212ea3)
![Alley Analysis 2](https://github.com/user-attachments/assets/d7229bc4-2ebc-4304-83fa-5fa92cf807df)

From this analysis, we confirm that the house is located on **Kenilworth Place**.





## we got it !! so the flag is : `IBOH24{Kenilworth_Place}`






