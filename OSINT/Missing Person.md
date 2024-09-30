# APU-IBOH24 Write-ups

## Missing Person OSINT Challenge

![Challenge Image](https://github.com/user-attachments/assets/39439c8c-2976-4db4-b105-91b513f27d4f)

### Challenge Overview

In this challenge, we were provided with a digital diary, which hinted at potential clues regarding the target's projects. The diary can be viewed here: [Digital Diary](https://lucasjalong.blogspot.com/2024/09/an-osint-enthusiasts-digital-diary.html).

Upon reviewing the diary, we noticed a suspicious line:  
*“Interested in my projects? Perform some OSINT tricks on me to find them yourselves. Prove your worth 😎”*

### Step 1: Identifying the Target's Projects

Just above this line, we found a list of the target's projects:

![Project List](https://github.com/user-attachments/assets/e00da886-e104-4a0c-ac0b-91f52e2c06fc)

Since many tech enthusiasts host their projects on GitHub, we decided to search for the target's GitHub profile. A quick look at the date the projects were uploaded (September 2024) and the diary’s date (also September 2024) led us to a repository named "BorneoShadow." This is crucial, as the target's blog mentions they are a native of Borneo. This alignment of details confirmed that we were on the right track.

![GitHub Profile](https://github.com/user-attachments/assets/72c25a7c-f1e5-49fe-8894-0a2d15bef901)

### Step 2: Analyzing the GitHub Repositories

Looking into the repositories, we found an interesting README file that said:

*“Join The Intelligence Den and learn! It's an excellent space for learning about OSINT, sharing insights, and collaborating with like-minded individuals. Mai berandau enggau kami!”*

This was followed by an invitation link to a Discord server:  
[Join The Intelligence Den](https://discord.com/invite/dYqyYMmeXa)

![README Snippet](https://github.com/user-attachments/assets/b019d61c-ab97-46df-a39d-cc533092117e)

### Step 3: Joining the Discord Server

After joining the Discord server, we noticed that most messages and channels names were encrypted using a cipher method. However, there was one public challenge titled "Verification."

![Verification Challenge](https://github.com/user-attachments/assets/4cda29d3-c2ca-42c2-b6fe-5ddde884e49e)

The challenge was straightforward: the bot asked for the user ID of the server owner. By observing the member list, we identified one user with a leader emoji beside their name, indicating they were the server owner. This gave us the required user ID.

![Discord Member](https://github.com/user-attachments/assets/b84eb5a4-fb4b-4d3d-9799-c304ef052b0e)

### Step 4: Unlocking the Cipher

Upon entering the correct user ID, a new channel was revealed. This channel contained the cipher and the decryption key:  
- Cipher: **Vigenère**
- Key: **shadowtrack**

![Cipher Information](https://github.com/user-attachments/assets/5342faf2-ba52-45c8-8d76-3fe3091f2b75)

### Step 5: Decrypting the Messages

We decrypted all messages and challenge names using the provided Vigenère cipher and key. However, most of the decrypted content led to false leads. After rethinking the situation, I realized that since the target encouraged us to join the Discord server via their GitHub profile, they must also be a member of the server.

By stalking the profiles of the server members, we identified our target's profile:

![Target Profile](https://github.com/user-attachments/assets/a39c6676-72e3-4122-a0af-88f8adfbfbb2)

From this profile, we found links to the target's GitHub account and X (formerly Twitter) account.

### Step 6: Analyzing the Target's X Account

On their X account, we found several tweets, some of which were encrypted using the same cipher we encountered earlier. One of these encrypted tweets contained a base64-encoded string at the end, indicated by the "==" padding.

![Encrypted Tweet](https://github.com/user-attachments/assets/68bb4398-31cf-4f48-b2fc-0e251c542ebf)

### Step 7: Decrypting the Tweet

We first decrypted the entire tweet using the Vigenère cipher, which revealed a base64 string:  
`SUJPSDI0e0sxZG40cHAzZF9pbl9LdWNoMW5nfQ==`

After decoding the base64 string using CyberChef, we got the flag:

![CyberChef Decoding](https://github.com/user-attachments/assets/83c6783e-ad1b-4689-b005-75f45b8efec8)

**Flag:** `IBOH24{K1dn4pp3d_in_Kuch1ng}`

---

### Lastly
The challenge was quite hard but also highly enjoyable to work on != :) 