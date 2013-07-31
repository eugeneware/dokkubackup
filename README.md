# dokkubackup

Backup all the [dokku](https://github.com/progrium/dokku) docker images on your system.

# Installation

Just copy `dokkubackup` to your PATH.

Ensure that `s3cmd` is install and in your PATH:

```
$ apt-get install s3cmd
```

# Usage

Make sure that you've configured `s3cmd` with your S3 credentials:

```
$ s3cmd --configure
```

The just execute dokkubackup passing in the name of your bucket

```
$ dokkubackup your.s3.bucket.name
```

This backs up the entire docker image and stores it in S3.

You may wish to run this as a cron job.

