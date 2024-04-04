#### list
- wsl -l -n
- wsl -l -o

#### install
- wsl --install [--distribution] [--no-launch] [--web-download] [--inbox] [--enable-- wsl1] [--no-distribution]

#### uninstall
- \<DistributionName\> config --default-user \<Username\>

#### set
- wsl --set-default \<Distribution Name\>
- wsl --set-default-version \<Version\>
- wsl --set-version \<distribution name\> \<versionNumber\>
\<DistributionName\> config --default-user \<Username\>

#### close
- wsl --shutdown
- wsl --terminate \<Distribution Name\>
- wsl --distribution \<Distribution Name\> --user \<User Name\>

#### check
- wsl --status
- wsl --version
- wsl --help
- wsl hostname -i

#### update
- wsl --update [--web-download]

#### run
- wsl --user \<Username\>

#### move
- wsl --export \<Distribution Name\> \<FileName\> [--vhd] [--version \<1/2\>]
- wsl --import-in-place \<Distribution Name\> \<FileName\>
- wsl --unregister \<DistributionName\>

#### mount/unmount
- wsl --mount \<DiskPath\> [--vhd] [--name] [--bare] [--type \<Filesystem\>] [--partition \<Partition Number\>] [--options \<MountOptions\>] 
- wsl --unmount \<DiskPath\>