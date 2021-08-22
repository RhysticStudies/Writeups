
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

![Alt text](https://github.com/RhysticStudies/Writeups/blob/PicoCTF/WhitePages/Screenshot3.png)

Converting the length of words into hex gives you.
696374667b415f73683072745f73743072795f69735f345f70696563655f6f665f70723073335f6631637431306e5f746861745f7479703163616c6c795f63616e5f62335f726561645f696e5f6f6e655f73697474696e675f5b2e2e2e5d7

![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/ICTF/Screenshot4.png)

Then converting that to words using cyber chef gives you the flag.

ictf{A_sh0rt_st0ry_is_4_piece_of_pr0s3_f1ct10n_that_typ1cally_can_b3_read_in_one_sitting_[...]}
