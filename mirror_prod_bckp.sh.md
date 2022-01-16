# Mirror Server/Production DB

    date=$(date +"%d%m%y")
    echo downloading backup date: $date...
    scp -i ~/.ssh/id_rsa root@IP_ADDRESS:PATH_TO_BCKP_FOLDER/project_db_${date}.sql LOCAL_PATH/project_db_${date}.sql
