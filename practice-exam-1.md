1. Create a new container secured Registry
2. Create public registery
3. Download CentOS 6 Image
4. Upload CentOS 6 Image
5. Create an image that installs Apache using CentOS 6
6. Uploads Apache Image Registry
7. Download verdaccio docker image
8. Upload verdaccio docker image to internal registry
9. Instantiate container from verdaccio, with port 4873
10. Create Docker Image from Apache image with an internal proxy to verdaccio container
11. Instantiate container from custom Apache image and link to verdaccio image
12. Upload Customer Image
13. Download mySQL docker Image
14. Create Docker image of snipeitapp, which is found https://snipeitapp.com/download
15. Instantiate mySQL container, with root password of "man@geASS3t!"
16. Instantiate snipeitapp docker image and link to mySQL container
17. Upload mySQL and snipeitapp image.
18. Create container volume.
19. Add index.html files to container volume.
20. Instantiate Apache container, mount volume container the index.html