Sample node.js app deployment with Ansible
===

Install ansible: [Ansible](http://docs.ansible.com/intro_installation.html)

Deploying app
--
```
cd deploy
ansible-playbook deploy.yml -i hosts -u root
```

## Private .env

Encrypt: `gpg -c .env`

Decrypt: `gpg -o .env -d .env.gpg`
