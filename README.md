- Install ansible
  - sudo easy_install pip
  - sudo pip install ansible

- Set remote server in hosts
  - `~/.ssh/config`
  
    ```
    Host my-hostname
    User ec2-user
    Hostname IP.IP.IP.IP
    IdentityFile ~/.ssh/key.pem
    ``` 
    
  - cf hosts file

- Move user pub key file in files directory
  - nomenclature `username.key.pub`

- Check users.yml settings

- Run `ansible-playbook -i hosts users.yml` to create users

- Try connecting to server in hosts file using new user private key
