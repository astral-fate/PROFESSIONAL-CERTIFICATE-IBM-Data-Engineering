
## Setting you local machine

1. [Installing Wget](#Installing-Wget)
2. [Installing Git](#Installing-Git)




# Installing Wget
wget is very helpful tool, it helps u import any set of data from any link and download it and work with it.
we can import cvs and JSON files and import them with wget. 

in this site, it provides us with number of JSON data that we can import using wget


https://jsonplaceholder.typicode.com/



make sure to install wget to work with importing files

https://eternallybored.org/misc/wget/

then after downloading  the exe file, copy and paste it to path
c/windows/system32/wget

and wooraa!!

<img width="648" alt="image" src="https://user-images.githubusercontent.com/63984422/184113637-36131bf3-7be9-4b37-b434-6cecaa51eaa2.png">
 
 now we can work it out in our Jubyter notebook
 
 <img width="892" alt="image" src="https://user-images.githubusercontent.com/63984422/184113712-d5942e8a-a7dd-4ab4-93c1-8b60e45ebbbe.png">


# Installing Git


to work with zip/unzip command, we have to install Git using this command 


       conda install git
       
<img width="767" alt="image" src="https://user-images.githubusercontent.com/63984422/184155684-e6f0b4af-e00c-4dc5-adeb-50f37c6c0f35.png">


then we can extract the files just fine 

<img width="763" alt="image" src="https://user-images.githubusercontent.com/63984422/184155839-dbc762f7-ccd7-4141-a1a3-b471101fdcae.png">


if we didn't install Git we will face error sayying: 

            'unzip' is not recognized as an internal or external command, operable program or batch file


There's another methods if we want to work with pakages, we have to first import a pakage named zipfile

         import zipfile
         
         
then we can write the follwoing function to extract the file 

        
           with zipfile.ZipFile("source.zip","r") as zip_ref:
                   zip_ref.extractall("targetdir")
                   


another method is by trying to download  7zip pakage from anaconda environmentm by this command

           
               conda install 7zip

<img width="881" alt="image" src="https://user-images.githubusercontent.com/63984422/184115908-e2d02e5d-da85-4aff-8d8d-b61e69adaea4.png">

<img width="772" alt="image" src="https://user-images.githubusercontent.com/63984422/184152586-212ee6cf-a069-42db-9d75-c9a2ab2b9674.png">



![image](https://user-images.githubusercontent.com/63984422/184123356-cef9bcf8-8a61-4cef-9d03-795dc795b8ba.png)


# Refences

1. https://www.youtube.com/watch?v=SE1nDEjER6Y&t=21s
2. https://anaconda.org/bioconda/p7zip
3. https://www.youtube.com/watch?v=7_o_kjG1Sfs
4. https://anaconda.org/conda-forge/unzip
5. https://notebooks.githubusercontent.com/view/ipynb?color_mode=auto&commit=f5441c90fe1994c4b7d025de76b331cb0155f149&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f676973742f417261736852617374692f38326265656465643830636131376234663639613061313835636430366564392f7261772f663534343163393066653139393463346237643032356465373662333331636230313535663134392f66696e616c5f61737369676e6d656e742e6970796e622e6970796e62&logged_in=false&nwo=ArashRasti%2F82beeded80ca17b4f69a0a185cd06ed9&path=final_assignment.ipynb.ipynb&repository_id=114696061&repository_type=Gist

