# KodeKloud Engineer Ansible

- Jumphost: `CentOS 8`

    - user: `thor`
    - password: `mjolnir123`

- Nautilus App Servers: `CentOS 7`

# Common Linux commands

| Service Name             | Command                     |
|--------------------------|-----------------------------|
| Nautilus App 1           | `ssh tony@172.16.238.10`    |
| Nautilus App 2           | `ssh steve@172.16.238.11`   |
| Nautilus App 3           | `ssh banner@172.16.238.12`  |
| Nautilus HTTP LBR        | `ssh loki@172.16.238.14`    |
| Nautilus DB Server       | `ssh peter@172.16.239.10`   |
| Nautilus Storage Server  | `ssh natasha@172.16.238.15` |
| Nautilus Backup Server   | `ssh clint@172.16.238.16`   |
| Nautilus Mail Server     | `ssh groot@172.16.238.17`   |
| Jenkins Server for CI/CD | `ssh jenkins@172.16.238.19` |

# SSH to server with sshpass

`sudo yum install sshpass -y`

| Service Name             | Command                                                                    |
|--------------------------|----------------------------------------------------------------------------|
| Nautilus App 1           | `sshpass -p Ir0nM@n ssh -o StrictHostKeyChecking=no tony@172.16.238.10`    |
| Nautilus App 2           | `sshpass -p Am3ric@ ssh -o StrictHostKeyChecking=no steve@172.16.238.11`   |
| Nautilus App 3           | `sshpass -p BigGr33n ssh -o StrictHostKeyChecking=no banner@172.16.238.12` |
| Nautilus HTTP LBR        | `sshpass -p Mischi3f ssh -o StrictHostKeyChecking=no loki@172.16.238.14`   |
| Nautilus DB Server       | `sshpass -p 'Sp!dy' ssh -o StrictHostKeyChecking=no peter@172.16.239.10`   |
| Nautilus Storage Server  | `sshpass -p Bl@kW ssh -o StrictHostKeyChecking=no natasha@172.16.238.15`   |
| Nautilus Backup Server   | `sshpass -p H@wk3y3 ssh -o StrictHostKeyChecking=no clint@172.16.238.16`   |
| Nautilus Mail Server     | `sshpass -p Gr00T123 ssh -o StrictHostKeyChecking=no groot@172.16.238.17`  |
| Jenkins Server for CI/CD | `sshpass -p j@rv!s ssh -o StrictHostKeyChecking=no jenkins@172.16.238.19`  |

# Getting Started

- Clone the repository: `git clone https://github.com/ntheanh201/kodekloud-engineer-ansible.git`
- Go to folder: `cd kodekloud-engineer-ansible`
- Install Ansible: `./install_ansible.sh`
- Solve task by running Ansible playbook

# Ansible

## Test environment

`ansible-playbook -i test-environments tasks/../solution.yaml`

## Nautilus environment

`ansible-playbook -i environments tasks/../solution.yaml`

# Tasks

- [Linux Timezones Setting](/tasks/linux-timezones-setting/)
- [Linux User Expiry](/tasks/linux-user-expiry/)
- [Linux User with Non-interactive Shell](/tasks/linux-user-with-non-interactive-shell/)
- [Linux User Without Home](/tasks/linux-user-without-home/)
- [Linux File Permissions](/tasks/linux-file-permissions/)
- [Selinux Installation](/tasks/selinux-installation/)
- [Linux Run Levels](/tasks/linux-run-levels/)
- [Create a Cron Job](/tasks/create-a-cron-job/)
- [Linux Postfix Troubleshooting](/tasks/linux-postfix-troubleshooting/)
- [Linux String Substitute](/tasks/linux-string-substitute/)
- [Linux User Files](/tasks/linux-user-files/)
- [Linux Remote Copy](/tasks/linux-remote-copy/)
- [MariaDB Troubleshooting](/tasks/mariadb-troubleshooting/)
- [Disable Root Login](/tasks/disable-root-login/)
- [Linux Services](/tasks/linux-services/)
- [Linux Banner](/tasks/linux-banner)
- [Linux Collaborative Directories](/tasks/linux-collaborative-directories/)
- [DNS Troubleshooting](/tasks/dns-troubleshooting/)
- [Linux NTP Setup](/tasks/linux-ntp-setup/)
- [Linux SSH Authentication](/tasks/linux-ssh-authentication/)
- [Linux Find Command](/tasks/linux-find-command/)
- [Linux LogRotate](/tasks/linux-log-rotate/)
- [Linux Configure sudo](/tasks/linux-configure-sudo/)
- [Web Server Security](/tasks/web-server-security)
- [Install a package](/tasks/install-a-package/)
- [Linux GPG Encryption](/tasks/linux-gpg-encryption/)
- [Configure Local Yum repos](/tasks/configure-local-yum-repos/)
- [Setup SSL for Nginx](/tasks/setup-ssl-nginx/)
- [Linux Bash Scripts](/tasks/linux-bash-scripts)
- [Application Security](/tasks/application-security/)
- [Apache Redirects](/tasks/apache-redirects/)
- [Add Response Headers in Apache](/tasks/add-response-headers-in-apache)
- [Linux Postfix Mail Server](/tasks/linux-postfix-mail-server/)
- [Create a group](/tasks/create-a-group/)