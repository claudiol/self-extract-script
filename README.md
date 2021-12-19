# self-extract-script
Template for Self Extracting Shell script

This small implementation can be used as a template to create a self-extracting script that can be used to install your software.

```
.
├── build
├── decompress
└── payload
    ├── files.tar
    └── installer
```

Files 
| File | Description |
| ----------- | ----------- |
| **build** | script that builds the self-extracting script |
| **decompress** | When ran, the script will remove the archive, decompress it and execute the install script we had created in the previous section |
| **payload/installer** | script contains any actions that you'd wish to be performed on the installation system, make directories, uncompress files, run system commands, etc. |
| **payload/files.tar** | File that contains all your software files |

This is the exact implementation from the [Linux Journal Article](https://www.linuxjournal.com/node/1005818). It has been usefule to me in the past
so I wanted to share it.
