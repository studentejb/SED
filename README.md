# SED
Use SED to vi a content into a file
exp.2 #sed -i '1i erik' passwdfile
exp.3 # sed -i '/student/a insert message' passwdfile
exp.3 #sed -i $'/Line to insert after/a\ i Line one to insert \\n
second new line to insert \\n
third new line to insert' file
add a line at the top of a file 

sed -i '1 i\line to be added ' file 

add a line at the top of a file 

sed -i '$ i\line to be added here'  file   

insert a line after a match

sed -i '/string match/a insert text here'   file 

insert a line at the line n 


sed -i 'ni avatar' file 

exple sed -i '6i enter your text here' file 

insert many line after a specific line 


sed -i $'/Line to insert after/a\ i Line one to insert \\n
second new line to insert \\n
third new line to insert' file

or 

sed -i $'/line to insert after/a\line1\\nline2\\nline3' file

Delete a line from a file
sed -i '/line to be deleted/d' file

insert lines after a match

sed -i '/pattern/a \line1 \line2'    inputfile

To apend the lines before:
 
sed -i '/pattern/i \line1 \line2' inputfile

Replace a line in a file
sed -i 'Ns/.*/replacement-line/' file.txt  ( N represent the line number .)

replace a string at a specific line

sed -i '34s/substituteAAA/withBBB/' file_name ( Note 34 is the line number.) # sed -i '2s/2 new/I did it/' passwdfile
