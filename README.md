# Plume4Windows

## Quick install

For those of you who do not want to spend almost 4 hours compiling Plume for Windows, here are the binaries needed for running the service using a SQLite or PostgreSQL database.

## Steps

1. Decide what database you will be using: sqlite or postgres
2. Extract "Plume_W64_v0.4.0_master-02c528c_postgres.7z" or "Plume_W64_v0.4.0_master-02c528c_postgres" to an easy place like `C:\Plume`
3. Modify the `.env` file to meet your needs
4. Run Migrations `plm migration run`
5. Initialise search index `plm search init`
6. Set up your instance `plm instance new`
7. Create admin account `plm users new --admin -n "adminusername" -N "Human Readable Admin Name" -b "Biography of Admin here" -p hackmeplease`
8. Create a task schedule to run Plume on system startup
9. Create a reverse proxy in IIS

## Other

Want to actually compile it yourself? See this [doc](https://github.com/Plume-org/docs/issues/82 "Install Plume on Windows").

## Last Updated

`Plume_W64_v0.4.0_master-02c528c_*.7z` was compiled from the "master" branch of [Plume](https://github.com/Plume-org/Plume/) and is up to date as of commit [02c528c](https://github.com/Plume-org/Plume/commit/02c528cae4385883d13bfff891d1656613d24edd) or January 29, 2020 03:37PM EST.
