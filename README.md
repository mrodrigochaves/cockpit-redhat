## Este é um tutorial de instalação e configração do Cockpit em distribuições Red Hat Enterprise Linux - RHEL.
---
Cockpit é uma ferramenta de interface gráfica web para servidores, destinada a todos, principalmente aqueles que desejam uma maneira fácil e gráfica de administrar servidores Linux.

# 💻 Stacks utilizadas:
![Cockpit](https://camo.githubusercontent.com/c357c39b244a01473099e0364bf20a68edda78929a3da840132bea7a30974f92/68747470733a2f2f696d672e736869656c64732e696f2f7374617469632f76313f7374796c653d666f722d7468652d6261646765266d6573736167653d436f636b70697426636f6c6f723d303036364343266c6f676f3d436f636b706974266c6f676f436f6c6f723d464646464646266c6162656c3d) ![Red Hat](https://img.shields.io/badge/Red%20Hat-EE0000?style=for-the-badge&logo=redhat&logoColor=white) ![Shell Script](https://img.shields.io/badge/shell_script-black.svg?style=for-the-badge&logo=gnu-bash&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
---

Instalação do Cokpit no Red Hat/CentOS/Fedora

`sudo yum install cockpit`

Ativar Cockpit:

`sudo systemctl enable --now cockpit.socket`

Abra o firewall se necessário:

`sudo firewall-cmd --permanent --zone=public --add-service=cockpit`

`sudo firewall-cmd --reload`

Depois que o Cockpit estiver funcionando, você poderá acessar os sistemas de todos os principais navegadores da Web em qualquer sistema operacional (incluindo Windows, MacOS e Android):

`https://ENDERECO_IP_DA_MAQUINA:9090`



![Cockpit Red Hat Painel](/cockpit-redhat.jpg)
Insira um usuário e senha válidos para logar no painel. 


---

### Para mais detlhes de como configurar o cockpit, acesse o site official do projeto clicando em [COCKPIT](https://cockpit-project.org/)