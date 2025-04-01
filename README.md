# Venmito_David_Velasquez

Name: David Velasquez\
Email : dav83@cornell.edu

# Requirements

1. Jupyter Notebook
2. Python 3
3. pandas, numpy, matplotlib, yaml, xml.etree.ElementTree, os, plotly.express


# Relevant Files

```Dataset```: Contains all of the new data files created from the code, formatted to match each other, and saved in the form of a CSV file\
```Venmito_David_Velasquez.ipynb```: The Jupyter Notebook containing the coding solution in three parts: data ingestion, data conforming and matching, data analyisis in the form of graphs, data output in text suggestions

# Solution Descriptions and Decisions
I decided to use Python. It is the most experienced language for me, but I do think OCaml would be a great language to use here as it naturally is used for data matching. I would've liked to use had it not been 5 years since I took the OCaml course from Cornell. I also used Jupyter Notebook as that is the platform Cornell emphasizes for its courses, and it is the easiest to run for a non-technical user. It also allowed me to combine my graphs and code into one file in a clear way. Jupyter is simple to use because it just requires a few downloads and a user can use it straight from their command prompt. The other nice thing is that Jupypter allows you to save it as a PDF with all the code ran already, making it so a user doesn't even need to run the code themselves if they were only interested in the final output. 

I structured the notebook based on the sections provided to me in the original READme file. I think it sections it into a great way to utilize the waterfall method of coding, another thing that is emphasized at Cornell. It allowed me to see what I still needed to work on in a clear way. I started with creating python functions to read each file type using Pandas. Pandas is widely used for data parsing, so it was a given. Once each function reads the file, it creates their respective Dataframe that will allow us to manipulate its contents and save it into a new csv file later on. 

For the matching and conforming section, I had to recognize patterns between all the files. I first started with people.json and people.yaml as they most closely were related to each  other. I had to combine.json first_name and last_name parameters to a single name paremeter to better fit with the yaml file that only had a name parameter. I then had to rename each parameter that was mismatched such as telephone to phone, city to location, and unmap 'devices' from .json to match .yaml. id also had to be changed to remove starting 0's, and changed to int to be able to manipulate. Finally everything was merged and moved around to create a concise table. the .xml file was fine by itself. the .csv files were difficult as I had to use my previous merged .json and .yaml to fill in the missing information of email and phone number. 

Finally, the data analysis. I used matplotlib as it is the only graphing package I used while I was at Cornell. I took a look at each file, found stats that I thought was most relevant, and made it into graphs for better visual output. The maximum of a graph was highlighted in a different color to be easily identifiable. These graphs then allowed me to make suggestions for Venmito.

# Future Improvemenets
I do recognize my coding is rather complex and long. SQL can for sure be used to minimize the amount complexity and brute force methods I used considering the solution uses a lot of table manipulation. I just have really no experience with SQL and was not something I was taught from Cornell. The only experience I had was a brief introduction I had based on the job description to be able to pass the coding assessment portion of this interview process. I also was unfortunate enough to be hit with a cold on the day I received this coding assigment, so naturally that affected the performance of my code. 

# File Instructions
Since I used Jupyter Notebook, it is rather easy to access and run. A user simply needs to download Juypter Notebook to their computer, download or fork this repository to a part of their computer, run command prompt, access the file location and run juypter notebook. Once in Jupyter Notebook, a user will need to download the relevant packages from python. Then, a user can run a cell one by one by selecting the block, then pressing the play button in the top menu. They can also run all cells in the same menu. 

