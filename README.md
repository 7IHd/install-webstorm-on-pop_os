# Install Webstorm on Pop!\_os
Not too straight forward. The download page says to extract the tar within an empty directory, but the actual documentation recommends to point to the `/opt` directory. If you extract it and then run it from where you extracted it, then webstorm cannot be moved without having to update various files that depend on the file path e.g. `.desktop` file.

Unpack the WebStorm-\*.tar.gz file you have downloaded to a different folder if your current Downloads folder doesn't support file execution:
```
tar xfz WebStorm-\*.tar.gz <new_archive_folder>
```

The recommended install location according to the filesystem hierarchy standard (FHS) is /opt. To install WebStorm into this directory, type the following command:
```
sudo tar xfz WebStorm-\*.tar.gz -C /opt/
```

Switch to the bin subdirectory:
```
cd opt/WebStorm-\*/bin
```

Run `webstorm.sh` from the bin subdirectory.
