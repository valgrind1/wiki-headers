# wiki-headers

A Python script that determines the most common words used in headers of wikipedia articles. Note that the headers are assumed to be surrounded by two equals signs, i.e. ==New York==

__Use:__
Simply change the following line of code: `SOURCE = "wiki_data.txt" #filename of dataset` to have the filename of the dataset you're going to use instead. i.e. `SOURCE = "<your_dataset_name>"`

__Additional Settings:__
Settings are currently from lines `12` through `16`
- adjust the _n_ most common words to display by changing the `OCCURENCES` variable. Default = `10`
- toggle program runtime display on/off by changing the `RUNTIME`. Default = `True`
- toggle including/ignorning subheaders in the final ranking by changing `SUBHEADERS`. Default = `False` 
- toggle if the words should be case-senstive by changing `CASE_SENSITIVE`. Default = `False`

__Sample Output:__
```
10 most common words in headers:
CASE_SENSITIVE = False
INCLUDE SUBHEADERS = False

RANK WORD           COUNT
-------------------------
1.   references     3527
2.   external       2506
3.   links          2503
4.   also           1113
5.   see            1112
6.   and            858
7.   history        766
8.   licensing      636
9.   summary        588
10.  career         548

--- runtime: 0.311229944229126 seconds ---
```
