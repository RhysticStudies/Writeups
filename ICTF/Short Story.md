CTF Name: Imaginary CTF
Problem Name: Short Story
Date: 7/31/21 
Problem Category: Forensics


When you first open the problem it gives you a .txt file to download where the flag is hidden.
![Alt text](https://github.com/RhysticStudies/Writeups/blob/main/ICTF/Screenshot1.png)

Opening the file with notepad gets you a list of random words that seem to have nothing in common. However, given the problem is Forensics we're likely dealing with Stegonargraphy. The information then should be hidden in the words somehow.

Under further examination you can see that there is a relationship between the length of the words all of them being 1-16 letters in length. So by reading in the file and taking the lengths of the words and treating them as hex you can find the nessage.

Converting the length of words into hex gives you.
696374667b415f73683072745f73743072795f69735f345f70696563655f6f665f70723073335f6631637431306e5f746861745f7479703163616c6c795f63616e5f62335f726561645f696e5f6f6e655f73697474696e675f5b2e2e2e5d7

Then converting that to words using cyber chef gives you the flag.

ictf{A_sh0rt_st0ry_is_4_piece_of_pr0s3_f1ct10n_that_typ1cally_can_b3_read_in_one_sitting_[...]}
