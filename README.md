# airfllow-datacamp

## Lnux Commands

- **Give all access to file/folder and all subfolders:**
  `sudo chmod -R 777 data_postgres`
- **Give all access to file/folder:**  
  `sudo chmod 777 data_postgres`
- **View History:**  
  `history`
- **Check OS Details:**  
  `cat /etc/os-release`
- **view all environment variable:**
  `env`
- **view environment variable with specific name:**
  `env | grep search_value`
- **Doenload a file using wget:**
  `wget -O sample_files/data.csv "https://cdn.wsform.com/wp-content/uploads/2020/06/color_srgb.csv"`
- **Difference btw -O vs -o:**
  `-O use to dowonload file content in shared path and -o saves logs in file`
- **Difference btw /folder/file.csv vs folder/file.csv:**
  `/ before folder means absolute path from root and without / means rlative path from pwd`
- **Download using curl:**
  `curl -o sample_files/datacurl.csv "https://cdn.wsform.com/wp-content/uploads/2020/06/color_srgb.csv"`
  `curl -o works as wget -O`
- **view all environment variable:**
  `env`
- **view all environment variable:**
  `env`
- **view all environment variable:**
  `env`

---

## Airflow Docker

- **SSH to airflow container:**
  `docker exec -it --user root  6147014504d9 /bin/bash`
- **Airflow file directory:**
  `/opt/airflow/output_files`
- **Copy file from container to local:**
  `docker cp 6147014504d9:/opt/airflow/airflow.cfg ./data/airflow.cfg`
  `docker cp 6147014504d9:/opt/airflow/airflow.cfg airflow.cfg`
- **build new image for airflow:**
  `docker build -t custom-airflow:latest .`
- **Download zip and extract to csv file:**
  `wget -qO- https://github.com/DataTalksClub/nyc-tlc-data/releases/download/green/green_tripdata_2019-01.csv.gz | gunzip > /opt/airflow/output_files/dataunzip.csv`
