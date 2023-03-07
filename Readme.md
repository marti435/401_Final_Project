#### **Streamer Feather Visualization using UTM Georeference Data** ####
##### **Emma Martin** #####



- ##### **Goals** #####
    - The visualization of streamer feathering above the Queen Charolette Fault using georeferenced UTM coordinates.
        - The reading in and interpolation of a p190 file in order to create streamer location reconstructions.


- ##### **Motivation** #####
    - My upcoming researh project is producing shot gathers for seismic tomography. Tomography often assumes that the streamer is staying straight in the water. By making these reconstructions we can determine the accuracy of shot-gathers based on the travel time to a curved streamer. 
    - Being able to read a p190 and pull the necessary information will allow for a more streamlined process in the future. 
        - Creating a standardized way to pull information out of a p190 file, based on indicators in the text, will allow for a more standardized way to read p190 files (there really isn't a set way yet).


- ##### **Data** #####
    - I am using a p190 file which is a streamer specific data file.
        - It contains information about the location of the streamer, shot number, and the UTM location of every hydrophone in the streamer.
    - The data I am accessing was sent to me directly from the research supervisor. Because of this direct access I am including the file in the GitHub Repository.
        - In theory the script should be able to read in any p190 file, but for accuracy I am including the file I used to create the script.


- ##### **Analysis Methods** #####
    - In the provided script I used dataframe associated operations.
        - This includes;
            - .chunk() - allows me to split the file up into smaller sections to be read individually. In the case of this file it is reading the file into chunks based on shot.
            - .append() - adds information pulled from the file and adds it to the data frame.
    - There was additional operations used to read in specific parts of the file to pull information from the file without putting it into a dataframe.
        - This includes;
            - .readlines() - pulls specific parts of a line based on its character position. 
            
            
- ##### **Take-Aways** #####
    - I have learned more about the importance of reading and understanding a file in order to create the best code you can. p190 files are very confusing so the fact that I had to dig in and find different points in the data really helped me to understand what information I was being given and what it meant. 
    - I also learned more about the process of pulling information from a file and adding it to a dataframe/list. The entire process I had to complete was mostly just figuring out where things were in a line so I could pull it more accurately. 
    - Additionally, I learned the importance of trial and error. throughout this course I was able to comeplete most of the problems given to me in very few tries so having to try things 100s of times really showed the importance of trying new things and experimenting to get the best outcome possible with what I wanted to do.


- ##### **References** #####
    - Andrew Gase, PhD, postdoctoral fellow
    - Emily Roland, PhD
    - Western Washington University Geology Dept.


