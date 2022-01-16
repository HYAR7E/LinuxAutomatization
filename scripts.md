# scripts
Random scripts i write to achieve work stuff or just to make my life easier



## Backup Notes-up database with GDrive
This requires:
- [Google Drive CLI Client](https://github.com/prasmussen/gdrive) script v2.1.1
- [Notes-Up](https://github.com/Philip-Scott/Notes-up) app v2.0.2

``` bash
gdrive sync upload --keep-local /home/USER/.local/share/notes-up GD_FOLDER_ID
```


## Start my workspace
[Script here](./start_workspace.sh.md)


## Mirror server backup file
[Script here](./mirror_prod_bckp.sh.md)
