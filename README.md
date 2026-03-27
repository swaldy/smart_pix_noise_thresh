Due to long run times, I actually ran multiple scripts at once to conserve time. My work flow went as follows. 

Since all the data parquet files were on CERNBox, I found it easier to just run preprocessing on lxplus. 
To make things run faster, I actually ran about 5 shells on lxplus at a time with multiple different scripts per the sensor geometry.
This can be found in the pre-processing folder. 
A larger script can be found which goes through all sensor geometries at once but only for one noise threshold which can be changed via hardcoding. 

I used the same logic for the NN running on the EAF facilities, meaning I ran two NN at a time. Each NN script has a different noise threshold. 
These scripts are found in the NN folder.

Next, data reduction is a much faster processes. This I still left hardcoded. 

Then lastly, paper plots give the final results. 
