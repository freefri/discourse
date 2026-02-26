Setup a dev environment instructions https://meta.discourse.org/t/install-discourse-for-development-using-docker/102009 

Start locally with a password and admin account like local_discourse@freefri.es `48urseoihj7fwe4uiy528734`

```
d/boot_dev --init
# wait while:
#   - dependencies are installed,
#   - the database is migrated, and
#   - an admin user is created (you'll need to interact with this)

# In one terminal:
d/rails s

# And in a separate terminal
d/ember-cli
```

Open the browser on http://localhost:4200

