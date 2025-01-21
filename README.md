# entryFilter
a simple code to filter entries in non-data-structured excel sheet

i've found the following task on r/slavelabour subreddit:

"I have this Google Sheet:
https://docs.google.com/spreadsheets/d/1j0PbcJOdmPrKL9pAF0XCzExiB64VaXsINDiPoj9ERXw/edit?usp=sharing
It contains 1,646 land listings.

Instructions:
Delete all land listings except the 481 listings that contain the word "vac".
Keep the first 11 lines of the file (header) intact – all other information can be removed.
A "land listing" includes the rows that begin with **** LISTING ID **** and end before the next listing starts."

took it to practice, didn't ever submit the solution.

Some commentary on the results:

i believe 'vac' stands for 'vacancy'. anyway, even though not specified, the sensible information seems to be the one in the second row after the identifier. however, the instruction asks for "contain the word vac". Entries 125.-1-15.112, 146.1-1-57 and 146.-1-7 were included, because they have names like "Novack John", which meet the criteria.

also, the instruction asks for 481 listings, but there are only 480 that meet the criteria. the difference happens becouse entry 144.-1-16.111 has the word vac on the important cell, but also has the name Kovacs Alex on a different cell. The employer probably counted the "vacs" in the document as a whole, without considering the possibility of a double match in the same entry.
