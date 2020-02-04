## Reverse Proxy using IIS

**Note**: I have yet to get this to work with a subdirectory. So, if your domain is https://mydomain.com, it can only work there and not at https://mydomain.com/plume as far as I am aware. If anyone figures this out, please let me know!

1. You need to have installed URL Rewrite (Figure 1)
2. From the Sites, choose your site, in the middle pane, double click URL Rewrite.
3. On right hand side, Add Rule, Blank Rule
4. Name it Plume with pattern (.*) with Action type Rewrite and Rewrite URL of http://127.0.0.1:7878/{R:1} (Figure 2)
5. Apply

| ![Plume_Win_IIS_01](https://user-images.githubusercontent.com/4871781/73027497-2aa79c00-3df9-11ea-93a1-5109b614a5e3.png) |
| :---: |
| **Figure 1** |

| ![Plume_Win_IIS_02](https://user-images.githubusercontent.com/4871781/73027553-3f842f80-3df9-11ea-99db-c9ecb88ae543.png) |
| :---: |
| **Figure 2** |