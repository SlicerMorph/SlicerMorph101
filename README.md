# SlicerMorph101
## Introduction to 3D Morphology with 3D Slicer and SlicerMorph

### Course Prerequisites

If you do not already have them, please obtain accounts at:
* https://github.com
* https://morphosource.org
* https://orcid.org.
  
GitHub and ORCID are mandatory to use MorphoCloud. MorphoSource account is required, if you want to be able to download data (you can search for data without an account). 
  
Also you will **need a 3-button mouse (cannot emphasize this enough)** to operate 3D Slicer (or any other 3D software) effectively. Optionally, [install a preview version of Slicer with a revision number 33550 or higher.](https://download.slicer.org) on your own computer as a backup, in case you have issues with cloud connections. 

Finally, having a second monitor is advised, since that will allow you to keep your zoom and cloud sessions on separate screens. 

### MorphoCloud On Demand
We will run this course through our cloud platform, MorphoCloud On Demand. Once you obtain the necessary accounts, to go https://instances.morpho.cloud, read the document about how MorphoCloud operates, and then use the provided link to request an instance. It is important that you do this **at least 24h before the course starts** to give enough time that your instance request to be approved, setup properly and for you to have a chance to test it. 
For ideal performance, we suggest using a wired ethernet connection at your university's campus. A dedicated wifi network (like your home) should also work fine. Please avoid public wifi access points due to unpredictable network performance.  

Some important points about MorphoCloud On Demand sessions:
* Always keep your data in the **MyData** storage volume. This is your persistent storage, data stored elsewhere may get deleted.
* You will have to extend your session approximately every 3.5h after your instance becomes online. Simply click `YES` when the popup window shows up. You can also extend your session for 4h anytime by clicking the "Extend Session" icon on your desktop. 
* Because the **instances automatically shelve themselves after 4h** (unless you extend it), **the next morning you will find your instance is offline**. Go to your specific issues page (direct link is in the email sent to you by MorphoCloud earlier), and type <br> ```/unshelve``` **to make your instance online again**. Based on the tasks in the queue, it may take anywhere from 2-20 minutes for your instance to become online. So make sure you do this before we start the course. Note that **all MorphoCloud commands are case-sensitive**, please make sure to type lower-case. 
* Use the `CTRL(CMD in Mac) + ALT + SHIFT` combination to make the cloud connection side window visible (or to make it disappear, if visible).
* For best user experience, switch to full screen mode in your browser window (not advisable if you do not have a second monitor, as you won't be able to see the zoom window).

#### MorphoCloud Desktop

**A:** Shortcuts to commonly used tools and applications. From left to right, minimize/maximize open applications, 3D Slicer, Terminal (aka shell console) window, File Browser, Firefox web browser, Application Search, File Browser. </br>
**B:** Right mouse clicking anywhere on desktop brings this menu, which lists all the applications and settings. </br>
**C:** Shortcut to your persistent storage volume, **MyData**. The actual folder is /media/volume/MyData. </br>
**D:** Side toolbar that gets activated by pressing the `CTRL (or CMD)` + `ALT` + `SHIFT` keys. It allows copy/paste into the remote session, browse and download files on the remote drive and adjust screen zoom levels (cut from the screenshot). </br>
<img src="https://github.com/SlicerMorph/SlicerMorph101/blob/main/MCI_Desktop.png" width=800>

#### Mapping the Sample Data Drive
To be able to access the drive with the preloaded workshop data, you need to execute this command in a terminal window:

```
curl https://jetstream2.exosphere.app/exosphere/assets/scripts/mount_ceph.py | sudo python3 - mount \
  --access-rule-name="MorphoCloudCephShare-ro" \
  --access-rule-key="AQAIDi1nKwbRFRAA9KKHUddANj6Ywj8ag7N9pg==" \
  --share-path="149.165.158.38:6789,149.165.158.22:6789,149.165.158.54:6789,149.165.158.70:6789,149.165.158.86:6789:/volumes/_nogroup/60bf684c-51d1-4abb-93f5-188d4d164111/1fe273cd-1e4d-4087-ad2b-01d548a16fe0" \
  --share-name="MorphoCloudCephShare"
```
This is a one-time setup, unless the instance has to be deleted and re-created. Share will be mapped to:

`/media/share/MorphoCloudCephShare`

and **it will be read-only**. You should continue saving your data into the your **MyData** folder (located in `/media/volume/MyData`)

#### Data transfer between your local computer and remote instance
**Uploading to remote:** If your files are small (<100MB) and you have a stable connection, just dragging and dropping individual files to the browser window. Those files will be saved under your **MyData** volume, which is located at `/media/volumes/MyData/`. If your data is already on the cloud (e.g., MorphoSource, dropbox, google drive, etc), the fastest way is to use the Firefox browser built into the instance and directly download them to your remote session. Just remember to copy them to your `MyData`. </br>
**Downloading from the remote:** If the file is small, you can use the interface shown above in the screenshot (Box D:), which works one file at a time. 

If you have many files, or your files are large, we advise to use SFTP (Secure FTP) tools for bulk upload/download. There are many free tools, search one for your computer. Remember, any data you have generated and important for you, you should download to your own computer. 

### Resources to use through out the course:

1. [Official Slicer User Manual](https://slicer.readthedocs.io/en/latest/)
2. [Official SlicerMorph Tutorials](https://github.com/SlicerMorph/Tutorials/)
3. [Slicer community forum](https://discourse.slicer.org)

### [Day 1](./Day_1.MD)

### [Day 2](./Day_2.MD)

### [Day 3](./Day_3.MD)

### [Day 4](./Day_4.MD) 
