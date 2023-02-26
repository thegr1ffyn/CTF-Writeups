# You Can't See Me |Steganography | Hamza Haroon

## Hint: [https://www.youtube.com/watch?v=2ctD30NNiEo](https://www.youtube.com/watch?v=2ctD30NNiEo&ab_channel=MEMES69)

[https://www.youtube.com/watch?v=2ctD30NNiEo&ab_channel=MEMES69](https://www.youtube.com/watch?v=2ctD30NNiEo&ab_channel=MEMES69)

## Solution:

The user is given a file named you_cant_see_me.jpg 

![You Cant See Me.jpg](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/You_Cant_See_Me.jpg)

Well, the image is of **Louis Braille**. Pretty simple to know if you know how to Reverse Search on Google Images.

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled.png)

Also, we check the strings of the image to see if we find anything useful. You can use HxD on Windows or strings on Linux. We are greeted with a ton of garbage values. So finding something useful is probably like a needle in haystack. 

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%201.png)

Notice that at the end of the file, some random 1’s and 0’s are given. Seems like something useful. Moreover, moving slightly above the last lines, we find ourselves a note. It seems like the given note is about how to decrypt the flag.

`QU9G{110000111000010100101110100110_101100100000101110_100100100000101110_010110101001100110110110100010_101110101010_100100101010111000101010111010011100}`

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%202.png)

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%203.png)

Notice how at the very start we got to know that the given image was of Louis Braille who designed the Braille language. 

Braille is a system of raised dots that can be felt with the fingertips and used to represent letters, numbers, punctuation, and other symbols. It was invented by Louis Braille, a Frenchman who was blind, in 1824. The Braille system uses a grid of 6 dots, with each dot being either raised or not raised, to represent a character. Each character is made up of a unique combination of raised dots within the grid and can be recognized by a person's sense of touch.

This is how Braille works

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%204.png)

The note tells us to move down the left column first. We can simply decrypt the flag by matching each bold dot to 1 and the other to 0 to find the flag. 

You can decode using this C++ code as well:

```cpp
#include <iostream>
#include <unordered_map>
using namespace std;

unordered_map<string, char> braille_map = {
    {"000000", ' '},
    {"100000", 'a'},
    {"110000", 'b'},
    {"100100", 'c'},
    {"100110", 'd'},
    {"100010", 'e'},
    {"110100", 'f'},
    {"110110", 'g'},
    {"110010", 'h'},
    {"010100", 'i'},
    {"010110", 'j'},
    {"101000", 'k'},
    {"111000", 'l'},
    {"101100", 'm'},
    {"101110", 'n'},
    {"101010", 'o'},
    {"111100", 'p'},
    {"111110", 'q'},
    {"111010", 'r'},
    {"011100", 's'},
    {"011110", 't'},
    {"101001", 'u'},
    {"111001", 'v'},
    {"010111", 'w'},
    {"101011", 'x'},
    {"101111", 'y'},
    {"101101", 'z'}};

string braille_to_text(const string &braille)
{
    string result;
    for (int i = 0; i < braille.size(); i += 6)
    {
        string braille_cell = braille.substr(i, 6);
        if (braille_map.count(braille_cell))
        {
            result += braille_map[braille_cell];
        }
        else
        {
            result += "?";
        }
    }
    return result;
}

int main()
{
    string braille = "INSERT ENCODED TEXT HERE";
    cout << braille_to_text(braille) << endl;
    return 0;
}
```

Or use [dcode.org](http://dcode.org) to find Braille Decoder:

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%205.png)

So we have our first part:

`blind_man_can_judge_no_colors`

To find the first part, simply decode using Base64 and you will find `AOF`

![Untitled](You%20Can't%20See%20Me%20Steganography%20Hamza%20Haroon%20b6a48fabe7fd41929c16d8004cc1bf05/Untitled%206.png)

So the final flag becomes:

`AOF{blind_man_can_judge_no_colors}`