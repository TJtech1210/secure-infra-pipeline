# Learning Notes

**Wed Nov  5 22:14:33 CST 2025:** Reviewed Python loop logic and counter.

---

**Sun Nov  9 20:45:00 CST 2025:** Added detailed notes on Terraform state files and ARNs.

## Terraform State File
- The `terraform.tfstate` file is Terraform's memory — it tracks what resources exist and their configurations.
- Never commit it to GitHub; it contains sensitive data like resource IDs and ARNs.
- Use a remote backend (S3 + DynamoDB) for safe, shared, and locked state storage.
- State locking prevents two applies from running at once and corrupting the state.

## ARNs (Amazon Resource Names)
- ARNs are AWS’s unique identifiers for every resource (buckets, instances, roles, etc.).
- Example: `arn:aws:s3:::tjtech-secure-infra` → an S3 bucket named `tjtech-secure-infra`.
- Avoid wildcards (`*`) in IAM policies — always use specific ARNs for least privilege and security.

