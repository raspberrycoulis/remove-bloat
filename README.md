# Remove Bloatware on the Raspberry Pi
Remove bloatware from Raspberry Pi Raspbian with one script. This will remove the storage hogging programs and some other often never-used tools including:

1. Wolfram Engine
2. LibreOffice
3. Minecraft Pi
4. Sonic Pi 
5. Dillo Web Broswer (dillo)
6. Image Viewer (gpicview)
7. Penguines Puzzle (penguinspuzzle)
8. Java (oracle-java8-jdk openjdk-7-jre oracle-java7-jdk openjdk-8-jre)

The script will then `autoremove`, `autoclean` and then `update` the aptitude pacakges on the Pi itself.

## Installation

### Automatic
Run the following command within the Raspberry Pi terminal:

```bash
sudo curl -fsSL https://raw.githubusercontent.com/raspberrycoulis/remove-bloat/master/remove-bloat.sh | bash
```

### Manual
If the automatic method does not work, you can manually download the repository and run the script after making it executable.

```bash
git clone git://github.com/raspberrycoulis/remove-bloat.git
cd remove-bloat
sudo chmod +x remove-bloat.sh
sudo ./remove-bloat.sh
```
