# ssh-login-alert
ssh-login-alert


sudo touch /etc/ssh/login_notify.sh

sudo chmod +x /etc/ssh/login_notify.sh

sudo nano /etc/ssh/login_notify.sh

selanjutnya

sudo nano /etc/pam.d/sshd
tambahkan yang ada tulisan #Login Telegram Notification seperti gambar



tambahkan di paling bawah

#Login Telegram Notification

session optional pam_exec.so /etc/ssh/login_notify.sh



ketik di terminal
PAM_TYPE="open_session" /etc/ssh/login_notify.sh



![image](https://github.com/agungsoboru/ssh-login-alert/blob/main/Screenshot%20(223).png)
![image](https://github.com/agungsoboru/ssh-login-alert/blob/main/Screenshot%20(129).png)
![image](https://github.com/agungsoboru/ssh-login-alert/blob/main/Screenshot%20(73).png)
