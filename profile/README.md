## Amphi: free, open-source tools for cloud IAM

![Amphi header](./amphi-header.png)

[Amphi](https://act.security/amphi) is a free collection of open-source tools for building, testing, understanding, converting, and managing cloud IAM policies.

Cloud access should not run on guesswork. Amphi helps security engineers and developers reason about what IAM policies actually mean, test access decisions before changes reach production, and understand effective access across real cloud environments.

---

## Tools in Amphi

### Author and understand policies

**[IAM Expand](https://github.com/act-security-labs/iam-expand)**  
See what wildcard actions actually grant by expanding patterns into the individual AWS actions behind them.  
[Open in Amphi](https://act.security/amphi/iam-expand)

**[IAM Shrink](https://github.com/act-security-labs/iam-shrink)**  
Compress IAM action lists to reduce policy size without changing the permissions they represent.  
[Open in Amphi](https://act.security/amphi/iam-shrink)

**[IAM Convert](https://github.com/act-security-labs/iam-convert)**  
Translate IAM policies between JSON and infrastructure-as-code formats.  
[Open in Amphi](https://act.security/amphi/iam-convert)

**[IAM Truth](https://github.com/act-security-labs/iam-truth)**  
Read policy conditions as truth tables so you can see which inputs produce an Allow or Deny.  
[Open in Amphi](https://act.security/amphi/iam-truth)

---

### Test and simulate access

**IAM Test**  
Build tests for IAM policy behavior and validate authorization logic before deploying it.  
[Open in Amphi](https://act.security/amphi/iam-simulate)

**[IAM Simulate](https://github.com/act-security-labs/iam-simulate)**  
Evaluate AWS authorization decisions locally, including the interaction between policies and IAM policy types.  
[Open in Amphi](https://act.security/amphi/iam-simulate)

---

### Understand effective access

**[IAM Collect](https://github.com/act-security-labs/iam-collect)**  
Collect policies, identities, resources, and other authorization data from AWS environments into a dataset that can be analyzed locally.  
[See it in Amphi](https://act.security/amphi)

**[IAM Lens](https://github.com/act-security-labs/iam-lens)**  
Explore effective access across IAM Collect data and answer questions like who can access a resource, what a principal can access, and why a request is allowed.  
[See it in Amphi](https://act.security/amphi)

---

## Amphi building blocks

The tools in Amphi are backed by open-source libraries, datasets, and automation that can be used directly in your own cloud security projects.

- AWS IAM action, resource, and condition-key data: [iam-data](https://github.com/act-security-labs/iam-data), [iam-data-go](https://github.com/act-security-labs/iam-data-go), [iam-data-python](https://github.com/act-security-labs/iam-data-python), [iam-harvest](https://github.com/act-security-labs/iam-harvest)
- IAM policy parsing and modeling: [iam-policy](https://github.com/act-security-labs/iam-policy)
- IAM simulation: [iam-simulate](https://github.com/act-security-labs/iam-simulate)
- IAM utilities and resource matching: [iam-utils](https://github.com/act-security-labs/iam-utils)
- CLI and developer libraries: [cli](https://github.com/act-security-labs/cli), [job](https://github.com/act-security-labs/job), [log](https://github.com/act-security-labs/log)
- Developer automation: [prettier-config](https://github.com/act-security-labs/prettier-config), [dual-npm-publish-action](https://github.com/act-security-labs/dual-npm-publish-action), [publishing](https://github.com/act-security-labs/publishing)

---

## Use Amphi wherever you work

- **In your browser:** use the free hosted Amphi tools.
- **In your terminal:** install the CLIs and compose them into scripts.
- **In your code:** use the underlying libraries to build IAM-aware applications.
- **In your pipelines:** test policies and access changes before they reach production.

---

## Contribute

Amphi is built in the open. If you find a bug, have an idea, or run into an IAM edge case we should support, open an issue or send a pull request in the relevant repository.

Cloud IAM has more than enough weird edge cases to go around.
