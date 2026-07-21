

  # AWS Cloud Cost Optimization - Identifying Stale Resources

 ## Identifying Stale EBS Snapshots
   
   In this example, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

### Description:

The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.


<img width="1920" height="1080" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/5c3818e4-4de4-4ebf-ae47-9ea5c2974bb1" />


<img width="1920" height="1080" alt="Screenshot (2)_LI" src="https://github.com/user-attachments/assets/6d64aecf-a8ff-4fd8-91d9-3dbcf6cb0fd6" />


<img width="1920" height="1080" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/5ef19723-49a9-41ee-851d-4edeb4e3e0dd" />


<img width="1920" height="1080" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/41709a12-40fc-47b2-91fa-52864ad0f0f1" />


<img width="1920" height="1080" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/01aa7fbf-f0b9-4307-8078-15c1a4c877d5" />


<img width="1920" height="1080" alt="Screenshot (7)_LI" src="https://github.com/user-attachments/assets/eebe455b-0fe7-4e71-b3ad-8a92577b3cb2" />

<img width="1920" height="1080" alt="Screenshot (8)_LI" src="https://github.com/user-attachments/assets/9bfc70c6-0ce1-4550-9ec5-dbce010ce9ed" />


