s# Introduction

## What is (L)FTP?

LFTP is a fast, free and open source, command line program for transferring files over FTP, the File Transfer Protocol. There are an incredible number of protocols for transferring files. Many of these can be used interchangeably, but some are best at certain tasks.

## Why not HTTP?

HTTP downloading is straightforward and easy: Tap an HTTP(S) download link in your favorite Web browser. Automating HTTP downloads is also relatively easy with curl/wget. If the files you want to download are few and small, HTTP is an efficient protocol for doing this.

## Why not BitTorrent?

BitTorrent is a fantastically efficient way to transfer and host files--big, small, thousands of them, or just a few! However, BitTorrent's peer-to-peer design can make it a bandwidth hog, starving the network of precious bandwidth. If your housemates enjoy playing online video games, or streaming video, you may want to investigate BitTorrent [seedboxes](https://en.wikipedia.org/wiki/Seedbox) to save bandwidth. If, on the other hand, you don't mind using all of your Internet speed, maybe you want to share your files publicly, BitTorrent is a great choice for transferring and hosting files.

## Why not SSH/SCP?

Secure Shell is another great tool for remotely accessing files and programs on remote systems. SSH is often used to administrate remote servers, while SCP is used to transfer files to and from SSH servers. SSH, SCP, and SFTP all use SSL to encrypt communication, but SSH/SCP are designed with secure remote execution in mind, while FTP is designed for faster file transfers. If you value secure, customizable sandboxes for running arbitrary commands, consider using SSH/SCP for transferring files.

## Why FTP?

If you want to use most of your bandwidth, while respecting other bandwidth-hungry applications; if you want to download files and folders; upload files and folders; securely and efficiently transfer files; only need a few user accounts; want to allow anonymous downloads; or, if the server that holds your files doesn't support other protocols; you might want to use FTP.

## Why LFTP?

Again, you have several choices. FTP files can be transferred by a variety of *FTP clients*. LFTP is a free and open source FTP client. LFTP is also one of the few FTP clients that offer *segmenting* for downloading files in parallel, making LFTP one of the fastest FTP clients available. LFTP uses a command line interface, making it more intensive to learn than graphical FTP clients. On the other hand, LFTP is fast and easy to automate. If you want fast, automated file transfer over FTP, LFTP is a top notch choice.

## Which protocols does LFTP support?

Some FTP clients support a handful of FTP/SFTP protocols. LFTP supports more than a handful of secure and insecure FTP and HTTP protocols:

* FTP
* SFTP
* FTPS
* FTPES
* FISH
* HFTP
* HTTP
* HTTPS