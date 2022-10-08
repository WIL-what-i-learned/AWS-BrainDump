# RDS - Backups & Recovery

- Automated Backups
    - daily
        - full backup stored in an a separate RDS owned bucket
    - every 5 min
        - transaction logs written to backup

- Manual Backups
    - kept until you delete them
    - use for checkpoints before large changes 
    - final copy before deleting a db

## Restoring Backup

- KEEP: parameter group & security group