alert_from_script
=================

Generate SNS alerts from any command.

Installation
============

::

$ sudo python setup.py install

Usage
=====

::

  usage: alert-from-script [-h] [--aws-access-key-id AWS_ACCESS_KEY_ID]
                           [--aws-secret-access-key AWS_SECRET_ACCESS_KEY]
                           sns_topic sns_subject script

  Runs a script and sends the stdout and stderr to SNS in case exit != 0.

  positional arguments:
    sns_topic             ARN of SNS topic to publish to.
    sns_subject           Subject used for SNS messages.
    script                The script to run. Includes all args to run.

  optional arguments:
    -h, --help            show this help message and exit
    --aws-access-key-id AWS_ACCESS_KEY_ID
                          Optional AWS Access Key Id. Will use environment
                          variables and instance profiles if not set.
    --aws-secret-access-key AWS_SECRET_ACCESS_KEY
                          Optional AWS Access Key Id. Will use environment
                          variables and instance profiles if not set.