# OTRS
To start the installation, download and run the pre-installation script;
su // root of law;
mkdir /gitSource //create folder;
cd /gitSource //in folder;
wget https://github.com/MAXPOL/OTRS/releases/download/preparation.sh/installOTRS.sh //download sh script;
chmod +x installOTRS.sh // give executable file permissions;
chmod 0777 installOTRS.sh //give full access rights;
./installOTRS.sh // start script;
//When you see the FINISH sign ..... proceed to the next step;
su otrs;
./Cron.sh start;
./otrs.Daemon.pl start;
//All OK GO http://ip_address/otrs/installer.pl;
