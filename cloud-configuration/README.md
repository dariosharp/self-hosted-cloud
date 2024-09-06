# Cloud Configuration
My cloud solution is composed of Nextcloud and Nginx for managing the application interface, Docker for managing applications easily, efficiently, and securely, and the combination of Ansible and Git for additional reliability. I chose to remove CasaOS from my Zimaboard and install Debian Stable to have full control over what is installed on the device.

# TOC
 - Cloud solutions comparison
 - Docker configuration
 - How to expose on the internet the cloud
 - Hardening

# Cloud solutions comparison
There are multiple applications for cloud interfacing. Most of them are very new and not completely mature but have potential. The most common applications are Nextcloud, Immich, PhotoPrism, and Piwigo.
- Nextcloud (https://nextcloud.com) is a cloud storage and collaboration platform that provides a wide range of functionality similar to commercial services like Google Drive or Microsoft OneDrive. It is well-designed for data protection, providing multiple encryption features. For example, it allows data to be encrypted per user, meaning that all files uploaded by a user are encrypted with their login password. Nextcloud can also be used for managing photos similarly to Google Photos or Apple iCloud. The web extension and the mobile application called "Memories" are very user-friendly and well-developed. Moreover, Nextcloud is stable, easy to update, and can be easily handled using Docker. Nextcloud also has a desktop application that automatically syncs directories. Overall, Nextcloud is a comprehensive, 360-degree cloud application.
- Immich (https://immich.app) is an open-source, self-hosted photo and video backup solution specifically designed to provide users with an alternative to services like Google Photos and Apple iCloud Photos. It is a relatively new project; thus, the mobile application does not properly upload images automatically when the application is in the background. Immich is well integrated with object recognition, which automatically detects objects and faces in images.
- PhotoPrism (https://www.photoprism.app) is an AI-powered photo management application that helps users organize, browse, and share their personal photo and video collections. It is designed to be a self-hosted alternative to commercial services like Google Photos, offering privacy, advanced search capabilities, and powerful AI-based features for tagging and organizing photos.
- Piwigo (https://piwigo.org) is a web-based photo gallery application designed for managing, organizing, and sharing photos and videos. It is a flexible and feature-rich platform that can be self-hosted on various types of servers, making it a popular choice for individuals, photographers, organizations, and businesses looking to have full control over their media libraries.
   
## Why NextCloud?
Nextcloud is very stable and has a visually appealing interface. The "Memories" application is very nice and offers a user experience similar to Google Photos. Personally, I prefer the UI of Nextcloud and Immich compared to PhotoPrism and Piwigo. However, Immich is still in its early stages; the mobile application does not automatically upload photos when running in the background, forcing users to constantly remember to open the app to start the photo upload process. In contrast, the Nextcloud app automatically uploads images in the background. Additionally, Nextcloud allows the upload of arbitrary files and can be used for collaborative environments.


