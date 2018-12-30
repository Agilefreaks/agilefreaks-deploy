AgileFreaks website deployment with Ansible
===

Install ansible: [Ansible](http://docs.ansible.com/intro_installation.html)

Deploying app
--
```
cd ./private
gpg -o .env -d .env.gpg
cd ..
ansible-playbook deploy.yml -i hosts -u root
```

## Private .env
cd into `./private`

Encrypt: `gpg -c .env`

Decrypt: `gpg -o .env -d .env.gpg`
