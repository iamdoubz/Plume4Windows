## Service Setup

### This is the preferred method of starting Plume on Windows

Once everything is working, you may be annoyed by having to always open a command prompt to start Plume. We can configure it to start on boot via Task Scheduler.

1. Open up the Task Scheduler app
2. On right hand side, choose Create Task
3. **General tab** - Name: "Plume"; Description: "Plume: a federated blogging application"; Run whether user is logged on or not; Run with highest privileges; Configure for Windows 10 (Figure 1)
4. **Triggers** - Begin the task At startup; Optionally Delay task for 30 seconds; Enabled (Figure 2)
5. **Actions** - Action: Start a program; Browse to plume.exe (default is C:\Users\%USERNAME%\.cargo\bin\plume.exe); Start in: C:\path\to\.env (Figure 3)
6. **Conditions** - Uncheck everything
7. **Settings** - Allow task to be run on demand; Run task as soon as possible after a scheduled start is missed; If the running task does not end when requested, for it to stop; Do not start a new instance

| ![Plume_Win_TS_01](https://user-images.githubusercontent.com/4871781/73027875-ec5eac80-3df9-11ea-8937-2d5335a5a882.png) |
| :---: |
| **Figure 1** |

| ![Plume_Win_TS_02](https://user-images.githubusercontent.com/4871781/73027475-18c5f900-3df9-11ea-8dbd-f7cc22088d5b.png) |
| :---: |
| **Figure 2** |

| ![Plume_Win_TS_03](https://user-images.githubusercontent.com/4871781/73027487-21b6ca80-3df9-11ea-986d-522731c82b01.png) |
| :---: |
| **Figure 3** |