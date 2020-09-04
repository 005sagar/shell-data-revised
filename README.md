# Shell-data-revised
In this project I will try to find which file has postive and negative comment using shell commands only.

## Get the .txt file in your project
* Go to the github link and click on the file name and click Raw it will give you a raw url and copy that url
* Open git bash and type curl and paste your url. Give it a name using > command
```curl https://raw.githubusercontent.com/denisecase/shell-data-processing/master/A.txt > firstfile.txt```
* Repeat same process for the another file 

## To process data
* Open git bash
* ``` $ grep "good" firstfile.txt``` this command will show you all the "good" string in that file, repeat with second file.
* ```$ grep -i "good" firstfile.txt``` -i will help you with case sensetive
* ```$ grep -i "good" firstfileA.txt - c``` - c command will count all the string "good". I got 36 on firstfile.txt and 18 on secondfile.txt
* Think different key word to find out which one will be postive and negative.

### Some Key word I tried
* ```$ grep -i "bad" firstfile.txt - c``` I got 4 on firstfile.txt and 58 on secondfile.txt
* ```$ grep -i "loved" firstfile.txt - c``` I got 10 on firstfile.txt and 0 on secondfile.txt
* ```$ grep -i "hate" firstfile.txt - c``` I  got 1 on firstfile.txt and 9 on secondfile.txt



