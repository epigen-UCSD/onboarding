# Guideline for  [virtural mechine](epigenomics.sdsc.edu)

## login 

1. login: `ssh username@epigenomics.sdsc.edu`
2. symlink data folder `ln -s /projects/ps-epigen/ ${HOME}/data`


## Share file via sFTP 
1. mv files into a folder (e.g. `xx_for_share`) under `/projects/ps-epigen/share/`
2. `sudo mount -o bind /projects/ps-epigen/share/xx_for_share /home/share_sftp/uid/xx_for_share` 
3. user login into `sftp uid@epigenomics.sdsc.edu` then can see the folder `xx_for_share`

## Share file via Personal links 
1. find `www` folder in your home folder. This is the web folder linked to address [http://epigenomics.sdsc.edu/your_user_id/]
2. put a blank index inside it; `> ${HOME}/www/index.html ` 
3. allow nginx to access: `chmod 0755 /home/$USER/www`
4. To share a folder in our data folder: `ln -s ${HOME}/data/folder_for_share ~/www/`; it should be able to be seen at [http://epigenomics.sdsc.edu/your_user_id/folder_for_share]

## Create users 

``` shell
adduser username
passwd usrname
usermod -g gname username
```

