# Introduction

What is LFTP? For that matter, what is *FTP*?

LFTP is a fast, free, command line program for transferring files over FTP, the File Transfer Protocol.

Why should you use FTP?

There are an incredible number of choices for downloading files. Most Web browsers get by with a simple tap to download files. Power users may enjoy BitTorrent for sharing public files. Others may prefer command line programs like curl and wget for automating multiple file downloads. Finally, at the bottom of the nerd spiral are FTP clients, for downloading folders and large bulk archives.

Many of these tools can be used interchangeably, but some tools are a better fit for certain tasks. FTP is a good fit for fast, private folder/bulk file transfers.

Why not BitTorrent?

BitTorrent is a fantastically efficient way to transfer files--big, small, thousands of them, or just a few! However, BitTorrent's peer-to-peer design can make it a bandwidth hog, clogging up the network from handling other bandwidth-hungry programs, like online video games. If you want to transfer files quickly, privately, and politely without hogging the network, FTP is a viable alternative. In fact, some BitTorrent users use both BitTorrent and FTP with *seedboxes*, seeding torrents on a remote "seedbox" server, and then transferring the files to a local computer with FTP. It's a great balance of speed and privacy!

That's a quick summary of why FTP is a good choice for transferring files. We will soon see why LFTP is a top choice compared to other FTP clients.

Why LFTP?

LFTP is an especially fast FTP client, one of the few that offer *segmenting* for downloading files in several parallel streams as once. LFTP offers a command line interface, making it harder to use than graphical FTP clients, but easier to automate.