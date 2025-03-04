# Pelatihan-Linux-2025
1. Mengunduh program wget,unzip, dan xxd, kemudian membuat folder baru bernama "artists_who_cam_sing" dan masuk ke dalam folder baru tersebut.
```bash
sudo apt install wget unzip xxd && mkdir artists_who_can_sing && cd artists_who_can_sing
```
2. Mengunduh file zip menggunakan wget
```bash
wget -O tutorials.zip "https://drive.usercontent.google.com/u/0/uc?id=1lV1HVmPTY_BOAK6ToXymRu7V5eVfR0ut&export=download"
```
3. Unzip file nya ke dalam folder baru yang bernama "singing_tutorials"
```bash
mkdir singing_tutorials &&  unzip tutorials.zip -d singing_tutorials
```
4. Mencoba masuk ke dalam folder "singing_tutorials" dan menampilkan list file nya termasuk yang tersembunyi
```bash
cd singing_tutorials && ls -la
```
5. Mencari tutorial “opera” yang dibuat oleh “NBAYoungboy” lalu memfilter semua tulisan dan  menampilkan satu baris yang berupa link yang benar, kemudian pipe hasilnya ke flag.txt di direktori "artists_who_can_sing"
```bash
find . -name "*_opera_*_NBAYoungboy*" | grep -rIh "FLAG{.*}" | head -n 1 > ../flag.txt
```
6. Masuk ke dalam folder "artists_who_can_sing" dann download sebuah file baru dengan ketentuan nama “plsrunmeiamnotmalwarefr”
```bash
cd .. && wget -O plsrunmeiamnotmalwarefr https://files.catbox.moe/9l4qu8 
```
7. Buatlah file tersebut dapat izin untuk execute dan menjalankan program tersebut
```bash
chmod +x plsrunmeiamnotmalwarefr 
```
8. Jalankan program tersebut menggunakan command di terminal linux
```bash
./plsrunmeiamnotmalwarefr && ps aux
```
9. Buat sebuah file bernama ransom.moonlah
```bash
touch ransom.moolah
```
10. Matikan procces tersebut dan pastikan bahwa program nya sudah mati
```bash
ps -o ppid= -p <pid> && kill -9 <ppid>






