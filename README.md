# Lab-03-Ensuring-Policies

## 📖 Summary
This lab demonstrates how to use Azure Policy to enforce governance within a resource group. We created three custom policies, grouped them into a policy initiative called **MapleTech Secure Foundation**, assigned it to a resource group, and tested various deployments to ensure compliance.

## 🛡️ Policies
1. **Only-CanadaCentral**  
   - **Effect:** Deny  
   - Restricts deployments to the Canada Central region.

2. **Require-ProjectName-Tag**  
   - **Effect:** Deny  
   - Ensures every resource includes a `ProjectName` tag.

3. **Deny-Public-IP**  
   - **Effect:** Deny  
   - Prevents creation of public IP addresses.

## 🎥 Video Demo
https://www.youtube.com/watch?v=gxVjpk23p7c&ab_channel=KarthikRaghavendraUrala

## 📸 Screenshots
Screenshots of policy definitions, initiative creation, assignments, and test case results are in the `/Ensuring policies` word doc.

## 📂 Policy Definitions
JSON files for all custom policies are stored in `/policy-definitions`.

## ✅ Challenges & Lessons Learned
- Ensuring JSON syntax was correct for each policy.
- Learned how initiatives simplify multi-policy assignments.
- Understood how Azure Policy evaluates resources at deployment time, preventing non-compliance.
