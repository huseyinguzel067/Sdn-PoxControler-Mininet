# Sdn-PoxControler-Mininet
Merhaba arkadaşlar bu uygulama pox controller , python ve mininet kulanılarak geliştirilmiştir . Bu yaptığım denemede projenin içinde yer alan sdn.png deki gibi bir topolojiyi işledim burda 4 host , 2 switch , 1  controler var mininetCode olan script ile 
topoloji oluşturuluyor ve controller olan scripte bu topolojinin içindeki switchlerin nasıl davranacağını planlıyoruz bu kuralara
flow deniliyor.Bu topolojide  vlan 10 ve vlan 20  iki farklı vlan var vlan içindeki hostlar sadece kendi aralarında  haberleşebiliyor . Bu sayade gereksiz broadcast trafiyi azaldı bu scriptleri çalıştırdığımızda h1 h4 ve h2 h3 ulaşabileceklerdir ama aynı network içerisinde olmalarına ramen h1 h3 veya h2 erişeyemeyecektir bu bizim scriptimizin çalıştığını göstermektedir.

Bu uygulamada ubuntu:16.04 üstunde yaptım minineti ubuntunun uzerinde kurdum 

    1  wget https://raw.github.com/mininet/mininet/2.2.2/util/vm/install-mininet-vm.sh
    2  bash -v install-mininet-vm.sh 2.2.2
    3  ~/mininet/bin/mn --version
    4  python mininet/examples/miniedit.py 
    
    
    bu komutları sirayla işlerseniz mininetiniz kurulmuş olacaktır. 4 satırda işlediyinizde de miniedit çalışacak yeni başlayan arkadaşlar için güzel bir uygulama miniedit mininet in görsel tarafıdır bazı durumlarda mininete  mininet root kullanıcısı eklemeseniz sıkıntı yaşayabilirsiniz  ben vlan yaplandırması kullandığımdan dolayı mininet  kullanmadım .
    
    
     Herkese iyi çalışmalar.

