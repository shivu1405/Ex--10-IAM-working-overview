# Ex-10: AWS IAM Working Overview

**NAME:** SHIVASRI  
**REG NO:** 212224220098

---

## Aim
To explore and configure AWS Identity and Access Management (IAM) users, groups, and policies, and to verify permissions for accessing Amazon S3 and Amazon EC2 resources.

---

##  Procedure
1. Start the AWS Lab and open the AWS Management Console.
2. Open **IAM** → **Users** and verify `user-1`, `user-2`, and `user-3`.
3. Open **User groups** and verify the groups **S3-Support**, **EC2-Support**, and **EC2-Admin** along with their attached policies.
4. Assign users to their respective groups:
   * `user-1` → **S3-Support**
   * `user-2` → **EC2-Support**
   * `user-3` → **EC2-Admin**
5. Open the IAM Sign-in URL and sign in as each user using the provided lab credentials.
6. **Test `user-1`:** Verify S3 access and confirm that EC2 access is denied.
7. **Test `user-2`:** Verify EC2 read-only access and confirm that attempting to stop an EC2 instance is denied; verify that S3 access is denied.
8. **Test `user-3`:** Open EC2, select `LabHost`, and stop the instance successfully.
9. Submit the lab and check the Grades/Submission Report.
10. End the lab after completing all tasks.

---

##  Output & Verification

<img width="1919" height="983" alt="Screenshot 2026-08-16 203731" src="https://github.com/user-attachments/assets/d8ec5761-ef75-4997-97aa-95b4601ee87e" />

<img width="1912" height="995" alt="Screenshot 2026-08-16 203741" src="https://github.com/user-attachments/assets/cae85656-6182-4bd3-9e62-bef7a2abc79e" />

<img width="1919" height="990" alt="Screenshot 2026-08-16 204334" src="https://github.com/user-attachments/assets/2c3e02db-1a09-4ed0-a635-380bb9373c99" />

<img width="1919" height="982" alt="Screenshot 2026-08-16 204625" src="https://github.com/user-attachments/assets/92994819-fc1f-42bd-a83c-33c4768bff9b" />

<img width="1919" height="979" alt="Screenshot 2026-08-16 204811" src="https://github.com/user-attachments/assets/6099fe58-82cd-4f08-a110-4847997f5d6d" />



---

## Result
The IAM users were successfully assigned to their respective groups, and the required permissions were verified:
* `user-1` successfully received S3 read-only access.
  <img width="1914" height="958" alt="Screenshot 2026-08-16 203916" src="https://github.com/user-attachments/assets/d2c02a72-6daf-43e8-a344-537640382eee" />

* `user-2` successfully received EC2 read-only access with modification restrictions.
  <img width="1919" height="951" alt="Screenshot 2026-08-16 203953" src="https://github.com/user-attachments/assets/83aca459-d1a7-46bf-96c1-1a749a01ace3" />

* `user-3` successfully received EC2 administrative access to manage instances.
 <img width="1919" height="961" alt="Screenshot 2026-08-16 204005" src="https://github.com/user-attachments/assets/440c794a-39a9-4768-83ee-8a44e73c47b6" />

  

Thus, IAM users, groups, policies, and permissions were successfully explored, configured, and tested.
