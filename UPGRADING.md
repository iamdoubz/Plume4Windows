# Upgrading

Choose the guide that is right for you, Postgres or SQLite.

## Postgres

1. Please make a backup of your database before continuing. There are many ways to export your database...

```
pg_dump -U username dbname > dbexport.sql
```

OR

```
sudo -u postgres pg_dump dbname > plume_backup.sql
```

OR

```
sudo -u postgres pg_dump -h localhost dbname > plume_backup.sql
```

Are a few examples.

2. Make a backup of your binary files.

```
xcopy /IK C:\Path\To\Plume C:\Path\To\Plume-bak
```

Or you can just right click, copy, right click, paste...

3. Download latest version and extract.

```
https://github.com/iamdoubz/Plume4Windows/raw/master/Plume_W64_v0.4.0_master-02c528c_postgres.7z
```

4. Stop the Windows Task Schedule.

5. Replace plm.exe and plume.exe with the new files.

6. Start the Windows Task Schedule. 

## SQLite

1. Please make a backup of your database before continuing.

```
copy C:\Path\To\Plume\plume.db C:\Path\To\Plume\plume.db.bak
```

2. Make a backup of your binary files.

```
xcopy /IK C:\Path\To\Plume C:\Path\To\Plume-bak
```

Or you can just right click, copy, right click, paste...

3. Download latest version and extract.

```
https://github.com/iamdoubz/Plume4Windows/raw/master/Plume_W64_v0.4.0_master-02c528c_sqlite.7z
```

4. Stop the Windows Task Schedule.

5. Replace plm.exe and plume.exe with the new files.

6. Start the Windows Task Schedule.