# 🔐 AWS IAM Security Implementation

## 📌 Project Overview
Hands-on lab implementing AWS Identity and Access Management (IAM) security best practices with focus on **least privilege principle**.

## 🎯 Objectives
- Create IAM users, groups, and roles with appropriate permissions
- Design and test custom IAM policies
- Implement role-based access control (RBAC)
- Understand IAM policy evaluation logic

## 📊 Architecture
![IAM Architecture Diagram](images/iam-architecture.png)


## 🛠️ Technologies & Services
- **AWS IAM**
- **AWS CLI** (for policy testing)
- **Python** (boto3 for automation - optional)
- **Terraform** (infrastructure as code - optional)


## 📁 Repository Structure

## 🚀 Implementation

### 1. IAM User & Group Structure
Created three-tier access model:
- **Admin Group**: Full access (with MFA required)
- **Developer Group**: Limited write access to specific services
- **ReadOnly Group**: View-only access for auditors

### 2. Custom Policy Creation
Designed policies that:
- Restrict actions to specific AWS services
- Limit resources using ARN patterns
- Include conditions (IP restrictions, MFA requirements)

### 3. Testing & Validation
- Used AWS CLI to simulate API calls
- Verified deny/allow outcomes match expectations
- Tested permission boundaries

## 🔐 Security Best Practices Applied
| Practice | Implementation |
|----------|----------------|
| Least Privilege | Minimal permissions per role |
| Separation of Duties | Distinct roles for different functions |
| Regular Audit | Policy versioning and review schedule |
| Multi-Factor Auth | MFA enabled for privileged users |
| Monitoring | CloudTrail logging enabled |

## 📈 Results
- Reduced unnecessary permissions by ~70% compared to default policies
- Clear audit trail for all IAM actions
- Scalable structure for team growth

## 🧠 Key Learnings
1. **Policy Evaluation Order**: Explicit deny > Allow > Implicit deny
2. **Service-Linked Roles**: Special roles for AWS services
3. **Permission Boundaries**: Limits maximum permissions
4. **IAM Access Analyzer**: Tool for policy validation

## 🔮 Future Enhancements
- [ ] Integrate with AWS Organizations
- [ ] Implement conditional policies with tags
- [ ] Automate policy reviews with AWS Config
- [ ] Add emergency break-glass procedures

---

## 👨‍💻 About the Author
**Renaldi**  
Cloud Security Learner | AWS Enthusiast  
[LinkedIn Profile](https://linkedin.com/in/yourprofile) | [GitHub Profile](https://github.com/renaldi136)

---
*Note: This project was completed as part of practical cloud security training.*
