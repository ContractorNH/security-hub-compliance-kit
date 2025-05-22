# Security Hub Compliance Kit

**Cross-account compliance at scale. Automatically enforced.**

This Terraform module enables AWS Security Hub, enrolls CIS and FSBP standards, and links member accounts for multi-account visibility and alerting.

---

## ✅ Features

- Enable Security Hub and CIS/FSBP controls
- Multi-account member enrollment
- SNS alert integration
- Modular design and reusable
- Compliant with AWS best practices

---

## ☁️ Tech Stack

- **Cloud**: AWS  
- **IaC**: Terraform  
- **Security Services**: Security Hub, Config, SNS

---

## 🚀 Usage Example

```hcl
module "security_hub" {
  source = "./modules/security_hub"

  enable_fsbp_standards = true
  enable_cis_standards  = true
  member_account_ids    = ["111111111111", "222222222222"]
  sns_topic_arn         = "arn:aws:sns:us-east-1:123456789012:SecHubAlerts"
  tags = {
    Environment = "prod"
    Owner       = "SecurityTeam"
  }
}
```

---

### [Deploy Compliance at Scale →](https://opscontractordev.super.site)

> Want access to the full Terraform deployment code?  
> Request private access at [your email] or through [your Super site].


*Generated on 2025-05-22 by The Contractor.*
