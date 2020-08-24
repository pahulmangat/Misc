import shutil 
import os

File_object = open("name.txt",'r') #name of text file
List =  File_object.readlines()
NewList = []
for x in List:
    NewList.append(x.replace('\n', ''))

src_dir = "C:\\src_dir" #name of folder where all files are
dst_dir = "C:\\dst_dir" #name of folder where you want files to go to

for i in range(0, len(List), 1):
    for file in os.listdir(src_dir):
        if file.startswith(NewList[i]):
            print('copying over: '+ str(NewList[i]))
            shutil.copy(src_dir + "//"+ file,dst_dir)
