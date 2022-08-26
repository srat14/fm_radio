# fm_radio
fm radio broadcasting with using Raspberry PI
// (Kullanılan kaynak:[https://circuitdigest.com/microcontroller-projects/raspberry-pi-fm-transmitter](https://circuitdigest.com/microcontroller-projects/raspberry-pi-fm-transmitter))
//Bu çalışmada RPİ ile radyo yayını yapacağız.
//RPI GPIO portunun 4 numaralı bacağına anten olması için jumper takarız.
//Programı ilk defa çalıştırmak için: İlk başta rpi üzerinde boş klasör oluştururuz.

mkdir fm // fm adlı klasör oluşturduk 
cd fm // ile fm klasörünün içine girelim
sudo git clone https://github.com/markondej/fm_transmitter// githubdan dosyaları çekeriz
sudo apt-get install gcc g++ make //ile programı yükleriz
cd fm_transmitter //fm transmitter dosyasının içine girip
sudo make //programı sudo make ile çalıştırırız.
sudo ./fm_transmitter -f 87.0 acoustic_guitar_duet.wav //ile fm transmitter dosyasından 87.0 frekanstaki dosyayı oynatırız.

//Artık bizde programlar yüklü olduğu için eğer tekrardan radyo yayını yapmak istiyorsak programı en baştan kurmamıza gerek yoktur. Yeniden radyomuzu çalıştırmak için:

//ilk başta fm_transmitter klasörünün içine girmeliyiz. ls ve cd kodlarıyla klasöre girdikten sonra:
sudo make // ile programımızı çalıştırdık
sudo ./fm_transmitter -f 87.0 acoustic_guitar_duet.wav // ile 87.0 dan radyo yayınını oluştururuz.
