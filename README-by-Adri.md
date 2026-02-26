# Dev
## Basic dev setup
Setup a dev environment instructions https://meta.discourse.org/t/install-discourse-for-development-using-docker/102009 

Start locally with a password and admin account like local_discourse@freefri `48urseoihj7fwe4uiy528734`

```bash
d/boot_dev --init
```
wait while:
  - dependencies are installed,
  - the database is migrated, and
  - an admin user is created (you'll need to interact with this)

In one terminal:

```bash
d/rails s
```

And in a separate terminal
```bash
d/ember-cli
```

Open the browser on http://localhost:4200 basic setup done.


### Useful commands

Shut down server with:

```bash
d/shutdown_dev
```

Open the container with:

```bash
d/exec bash
```

Open rails console:

```bash
d/rails c
```

Reset the database:

```bash
d/rails db:environment:set RAILS_ENV=development
d/rails db:drop
```

