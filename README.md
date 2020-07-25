To install dependencies:

- ```ansible-galaxy install -r requirements.yml```

To launch the playbook:

- ```ansible-playbook ./site.yml -i inventory --ask-vault-pass```

To deploy a new version of the application:

- ```ansible-playbook ./site.yml -i inventory --ask-vault-pass --tags deploy```

Add this to your ```ansible-playbook``` command if you want to update rust on the server:

- ```--extra-vars "upgrade_rust=yes"```
