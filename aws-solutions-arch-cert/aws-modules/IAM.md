# IAM 101

## Features

    Centralised control of you AWS account

    Shared Access to you AWS account

    Granular Permissons

    Identity Federation (Active Directory, Facebook, Linkedin, etc)

    MultiFactor Authentication

    Provide temporary access for users/devices and services where necessary

    Allows you to set up your own password rotation policy

    Integrates with many different AWs services

    Supports PCI DSS Compliance

## Key Terminology For IAM

    1. Users - End Users such as people, employees, etc.
    2. Groups - A collection of users. Each user in the group will inherit the permissions of the group
    3. Policies - made up of documents, called Policy documents. These documents are in a format called JSON and they give permissions as to what a User/Role/Group is able to do
    4. Roles - You create roles and then assign them to AWS Resources

## Exam Tips

    IAM is universal - does not apply to regions

    Root Account is simply the account created when first setup your AWS account it has complete admin access

    New Users have no permissions when first created

    New Users are assigned Access Key ID & Secret Access Keys when first created

    These are not the same as a password. You cannot use the Access key ID & Secret Access Key to Login to the console. You can use this to access AWS via the API and Command Line, however

    You only get to view these once

    Always setup MFA on root account

### Labs for cloud guru

    1. LAB: Add MFA to root

    QR can let you redo MFA

    Add User - access key and password console access

    Create Developer group - gave AdminAccess (Job Function)

    Added user to developer group

    AdminAccess 

    Effect: Allow

    Action: *

    Roles govern services (EC2 to admin access s3, etc)

    2. Create A Billing Alarm - LAB

    Create a billing alarm for 10 dollars - sends an email when bill goes over 10

    go into your email and subscribe to that topic

    Exam - how do you get notifications and that's through alarms
