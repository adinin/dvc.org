# Save Data

Now, that our data files are managed by DVC (see
[Add Files](/doc/get-started/add-files)) and to push data files from your
machine to the default [remote](/doc/commands-reference/remote) storage:

```dvc
    $ dvc push
```

The same way as with Git remote, it ensures that your data files and your models
are safely stored remotely and shareable. It means that this data could be
pulled by your team or you when you need it.

Usually you run it along with `git commit` and `git push` to save changes to
`.dvc` files to Git.

See `dvc push` for more details and options for this command.

**Internals:** you can check now that actual data file has been copied to the
remote we created in the [configuration](/doc/get-started/configuration)
chapter:

```dvc
    $ ls -R /tmp/dvc-storage
        /tmp/dvc-storage/a3:
        04afb96060aad90176268345e10355
```
