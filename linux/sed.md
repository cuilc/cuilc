for the first line:  
	sed -i '1i\'"$FirstLine" $Filename

for the last line:  
    sed -i '$ a\'"$Lastline" $Filename 