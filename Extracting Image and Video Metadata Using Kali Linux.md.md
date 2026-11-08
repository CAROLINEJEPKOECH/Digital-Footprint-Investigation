Extracting Image and Video Metadata using Kali Linux

1.##Introduction
Metadata is data about data. In images and videos, it tells where it was taken, what phone and Camera was used and sometimes where it was taken


2.##Installation
I had previously installed Exiftool package that is used to record the metadata.I therefore run the version of the exiftool present. Below is the screen shot for reference
(Installation Screenshot.png)


3.### Image analysis
This is my First JPEG Image i analysed. Full extracted record of it is saved in (IMG_20190907_170428_metadata.txt)  
File Name                       : IMG_20190907_170428.jpg
File Modification Date/Time     : 2021:02:28 00:09:59+03:00
File Access Date/Time           : 2026:11:05 17:19:28+03:00
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
Exif Byte Order                 : Little-endian (Intel, II)
Image Description               : 
Make                            : TECNO
Camera Model Name               : TECNO K7
Date/Time Original              : 2019:09:07 17:04:29


### Second Jpeg Analysis
File Name                       : Image 3.jpg
File Modification Date/Time     : 2021:02:28
File Permissions                : -rwxrwx---
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
X Resolution                    : 1
Y Resolution                    : 1
Image Width                     : 1280
Image Height                    : 960
The full extracted text files are saved in my files folder as (Image 3_metadata.txt)



4.### PNG Analysis
I analysed i PNG image (Image 4.png) using the Exiftool to check its metadata. The key findings from analysis are as below
File Name                       : Image 4.png
File Size                       : 25 MB
File Modification Date/Time     : 2026:11:05 23:27:17+03:00
File Access Date/Time           : 2026:11:05 23:37:30+03:00
File Type                       : PNG
File Type Extension             : png
MIME Type                       : image/png
Image Width                     : 3120
Image Height                    : 4160
The full text file containing all extracted metadata is saved im my files folder as Image 4_metadata.txt



5.#### GPS Investigation
-I checked the image metadata files to search for location data.
-GPS metadata was absent in 1 JPEG image (Image 3.jpg) and the PNG image (Image 4.png). this means that there was no location coordinates impedded in the images.
-I found GPS metadata i 1 JPEG file (IMG_20190907_170428.jpg). The GPS coordinates was detected showing;
Scene Capture Type              : Standard
GPS Version ID                  : 2.2.0.0
GPS Latitude Ref                : North
GPS Longitude Ref               : East
GPS Altitude Ref                : Above Sea Level
GPS Time Stamp                  : 14:04:29
GPS Processing Method           : FUSED
GPS Date Stamp                  : 2019:09:07



6.#### Video Analysis
-I analysed 1 MP4 video using Exiftool to inspect its embedded metadata.
-Below are key findings:
File Name                       : VID-20210923-WA0005.mp4
File Modification Date/Time     : 2021:10:01 20:59:47+03:00
File Access Date/Time           : 2026:11:05 16:48:34+03:00
File Type                       : MP4
File Type Extension             : mp4
MIME Type                       : video/mp4
Duration                        : 0:02:51
Avg Bitrate                     : 787 kbps
-The full extracted video metadata textfile is saved in my files folder (VID-20210923-WA0005_metadata.txt)



7.#### File Integrity
-I calculated the SHA-256 hash values for my evidence files to verify their integrity and ensure that they have net been altered
-File Image Hash value: 911102be339cfa7d7fddeaf8468f35107a5409bcc187879ecc80f648610a71c9 IMG_20190907_170428.jpg
-File Video Hash value:
8f3fbf371b8d1796ac050385c86d2bb96a2827ad982f9a4fe56ab19e4e5bc6a2b VID-20210923-WA0005.mp4



8. #### Reflection
-This investigation successfully demonstrated the process of extracting and analysing MetaData from images and videos ising Exiftool in Kali Linux.
-I learned how embedded Metadata reveals creation timestamps and file formats, how to check for privacy elements like gps data, and how to use SHA-256 hashes to verify file integrity
