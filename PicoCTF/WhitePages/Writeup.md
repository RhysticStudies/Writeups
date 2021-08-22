
CTF Name: PicoCTF  
Problem Name: White Pages  
Date: 8/20/21   
Problem Category: Forensics  
point value: 250  


When you first open the problem it gives you a .txt file to download where the flag is hidden.

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot1.png)

Opening the file with notepad gets you a seemingly blank notepad, however you can highlight text on it.

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot2.png)

Opening up the file using a hex editor you can see that the file actually contains some characters. There change at irregular intervals with some clear patterns.

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot3.png)

Using Find Replace and changing the first character with 0s you get,

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot4.png)

REplacing the other character with 1 you get,

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot5.png)

That's a Binary number. Converting that to Ascii you get the flag.

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/PicoCTF/WhitePages/Screenshot6.png)

picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}
