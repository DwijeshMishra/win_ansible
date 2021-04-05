

Gcp Windows Machine run this on Power shell
-----------------------------------------------------------------------------------------------------------------
$url = "https://raw.githubusercontent.com/ansible/ansible/devel/examples/scripts/ConfigureRemotingForAnsible.ps1"
$file = "$env:temp\ConfigureRemotingForAnsible.ps1"
(New-Object -TypeName System.Net.WebClient).DownloadFile($url, $file)
powershell.exe -ExecutionPolicy ByPass -File $file
winrm enumerate winrm/config/Listener
winrm set winrm/config/service '@{AllowUnencrypted="true"}'


Ubuntu 
sudo vim /etc/ansible/hosts

[win]
public ip

mkdir /etc/ansible/group_vars
sudo chmod -R 777 /etc/ansible/


vim /etc/ansible/group_vars/win.yaml

---

ansible_user: ansible

ansible_password: ansible

ansible_connection: winrm

ansible_winrm_server_cert_validation: ignore

ansible_winrm_transport: basic

ansible_winrm_port: 5985

ansible_python_interpreter: C:\Users\geekflare\AppData\Local\Programs\Python\Python37\python



