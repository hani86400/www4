# www4



 [https://hani86400.github.io/www4](https://hani86400.github.io/www4)

#### URL:
```
https://hani86400.github.io/www4

https://{owner}.github.io/{repo}
```

#### API:
```
curl -s -L -H "Accept: application/vnd.github+json" -H "Authorization: Bearer $GITHUB_TOKEN " -H "X-GitHub-Api-Version: 2022-11-28"  https://api.github.com/repos/hani86400/www4/git/trees/main?recursive=0 
```
#### OUTPUT:
```
{
  "sha": "8abbe9d80377961616d58616a0019e9a95546944 ",
  "url": "https://api.github.com/repos/hani86400/www4/git/trees/8abbe9d80377961616d58616a0019e9a95546944",
  "tree": [
    {
      "path": "AC",
      "mode": "100644",
      "type": "blob",
      "sha": "bf23b14d9875573a55d623ffbfaf888d84619d69",
      "size": 287,
      "url": "https://api.github.com/repos/hani86400/www4/git/blobs/bf23b14d9875573a55d623ffbfaf888d84619d69"
    },
    {
      "path": "README.md",
      "mode": "100644",
      "type": "blob",
      "sha": "0a0b8f9a1d928a1c201759dbe838dd0401fabcc5",
      "size": 7,
      "url": "https://api.github.com/repos/hani86400/www4/git/blobs/0a0b8f9a1d928a1c201759dbe838dd0401fabcc5"
    },
    {
      "path": "files",
      "mode": "040000",
      "type": "tree",
      "sha": "2f9fb1d53dffc326aaf4ee149d2bebb04ed5c51b",
      "url": "https://api.github.com/repos/hani86400/www4/git/trees/2f9fb1d53dffc326aaf4ee149d2bebb04ed5c51b"
    },
    {
      "path": "files/f1.txt",
      "mode": "100644",
      "type": "blob",
      "sha": "516fad407fa15aed56b6975c617c17536aaba032",
      "size": 9,
      "url": "https://api.github.com/repos/hani86400/www4/git/blobs/516fad407fa15aed56b6975c617c17536aaba032"
    }
  ],
  "truncated": false
}

```



#### PUTTY:
```
PUTTY_VER='0.80'
for   PUTTY_ARC in 'w32' 'w64' 'wa32' 'wa64'
do 
for   PUTTY_FILE in 'putty.exe' 'pscp.exe' 'psftp.exe' 'puttytel.exe' plink.exe' pageant.exe' 'puttygen.exe' 'pterm.exe' 'putty.zip' 
do
wget -c -O ${PUTTY_ARC}_${PUTTY_FILE}     https://the.earth.li/~sgtatham/putty/${PUTTY_VER}/${PUTTY_ARC}/${PUTTY_FILE}
wget -c -O ${PUTTY_ARC}_${PUTTY_FILE}.gpg https://the.earth.li/~sgtatham/putty/${PUTTY_VER}/${PUTTY_ARC}/${PUTTY_FILE}.gpg
gpg --auto-key-retrieve --verify ${PUTTY_ARC}_${PUTTY_FILE}.gpg ${PUTTY_ARC}_${PUTTY_FILE} 
done #PUTTY_FILE
done #PUTTY_ARC


for   PUTTY_FILE in 'puttydoc.zip' 'putty.chm'
do
wget -c -O ${PUTTY_FILE}     https://the.earth.li/~sgtatham/putty/latest/${PUTTY_FILE}
done #PUTTY_FILE

```



#### Windows Firewall:
```

REM To Turn Off:
NetSh Advfirewall set allprofiles state off

REM To Turn On:
NetSh Advfirewall set allprofiles state on

REM To check the status of Windows Firewall:
Netsh Advfirewall show allprofiles
```










