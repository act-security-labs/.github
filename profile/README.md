# Act Security Labs

### Open-source tools for understanding and securing cloud access.

Cloud access shouldn't run on guesswork.

**Act Security Labs** is the open-source engineering home of [Act Security](https://act.security/). We build tools, libraries, data, and experiments that help security engineers and developers understand how cloud access works, reason about what policies actually mean, and make safer changes with confidence.

Everything here is built in the open and available for the community to use, inspect, extend, and contribute to.

---

## The open arena for cloud access

Cloud authorization gets complicated fast.

A single access decision can depend on identities, resources, policies, organization guardrails, conditions, sessions, tags, and the relationships between them. Understanding what _should_ happen is difficult enough. Understanding what _will_ happen across a real cloud environment is harder.

We build tools that make those problems easier to reason about.

Our work focuses on a few core ideas:

- **Make access understandable.** Turn complex authorization logic into answers humans can reason about.
- **Test before you deploy.** Give engineers a way to understand the effect of a policy change before it reaches production.
- **Work from effective access, not configuration alone.** What matters is what an identity can actually do to a resource.
- **Build useful primitives.** Publish the parsers, datasets, simulators, and libraries that make better security tooling possible.
- **Build in the open.** Security gets better when practitioners can inspect the tools, challenge assumptions, and improve them together.

---

## Tools for the cloud access lifecycle

### Author and understand policies

Working with IAM policies shouldn't require manually decoding JSON and hoping you interpreted AWS correctly.

Our tools help you inspect, transform, and reason about policies before they ever reach an account.

**[IAM Expand](https://github.com/act-security-labs/iam-expand)**  
See what wildcard actions actually grant by expanding patterns into the individual AWS actions behind them.  
[Try it in Amphi](https://act.security/amphi/iam-expand)

**[IAM Shrink](https://github.com/act-security-labs/iam-shrink)**  
Compress IAM action lists to reduce policy size without changing the permissions they represent.  
[Try it in Amphi](https://act.security/amphi/iam-shrink)

**[IAM Convert](https://github.com/act-security-labs/iam-convert)**  
Translate IAM policies between formats used by tools such as Terraform, CloudFormation, and CDK.  
[Try it in Amphi](https://act.security/amphi/iam-convert)

**[IAM Truth](https://github.com/act-security-labs/iam-truth)**  
Turn complex policy conditions into something you can reason about, including the combinations of inputs that produce an Allow or Deny.  
[Try it in Amphi](https://act.security/amphi/iam-truth)

---

### Test and simulate

Policies are code. We think you should be able to test them like code.

**IAM Test**  
Build tests for IAM policy behavior and validate authorization logic before deploying it.  
[Try it in Amphi](https://act.security/amphi/iam-simulate)

**[IAM Simulate](https://github.com/act-security-labs/iam-simulate)**  
Evaluate AWS authorization decisions locally, including the interaction between different policies and IAM policy types.  
[Try it in Amphi](https://act.security/amphi/iam-simulate)

---

### Understand effective access

Configuration tells you what policies exist. Effective access tells you what they actually allow.

**[IAM Collect](https://github.com/act-security-labs/iam-collect)**  
Collect policies, identities, resources, and other authorization data from AWS environments into a dataset that can be analyzed locally.  
[See it in Amphi](https://act.security/amphi)

**[IAM Lens](https://github.com/act-security-labs/iam-lens)**  
Explore effective access across that data and answer questions such as:  
[See it in Amphi](https://act.security/amphi)

- Who can access this resource?
- What can this principal access?
- Why is this request allowed?
- Which policies contribute to this access?

---

## The building blocks

Not everything we build is an end-user tool.

Act Security Labs also publishes the libraries and datasets we use to work with cloud authorization programmatically.

You'll find projects covering areas such as:

- AWS IAM actions, resources, and condition keys: [iam-data](https://github.com/act-security-labs/iam-data), [iam-data-go](https://github.com/act-security-labs/iam-data-go), [iam-data-python](https://github.com/act-security-labs/iam-data-python), and [iam-harvest](https://github.com/act-security-labs/iam-harvest)
- IAM policy parsing and modeling: [iam-policy](https://github.com/act-security-labs/iam-policy)
- Policy evaluation and simulation: [iam-simulate](https://github.com/act-security-labs/iam-simulate)
- ARN and resource matching: [iam-utils](https://github.com/act-security-labs/iam-utils)
- IAM action expansion and minimization: [iam-expand](https://github.com/act-security-labs/iam-expand) and [iam-shrink](https://github.com/act-security-labs/iam-shrink)
- Cloud authorization data collection and analysis: [iam-collect](https://github.com/act-security-labs/iam-collect) and [iam-lens](https://github.com/act-security-labs/iam-lens)
- Reusable TypeScript libraries: [cli](https://github.com/act-security-labs/cli), [job](https://github.com/act-security-labs/job), and [log](https://github.com/act-security-labs/log)
- GitHub Actions and developer automation: [prettier-config](https://github.com/act-security-labs/prettier-config), [dual-npm-publish-action](https://github.com/act-security-labs/dual-npm-publish-action), and [publishing](https://github.com/act-security-labs/publishing)

If you're building your own cloud security or IAM tooling, these projects are intended to be useful building blocks.

---

## Research and experiments

Some access problems don't have good answers yet.

Act Security Labs is also a place for us to explore ideas that may begin as experiments rather than finished products.

That includes work around:

- large-scale cloud authorization analysis
- effective access and reachability
- least-privilege analysis
- authorization policy semantics
- access graph modeling
- organization-level cloud governance
- AI and agent authorization
- new ways to analyze and enforce cloud access boundaries

When we build something useful, we'd rather put it in the hands of practitioners and learn together.

---

## From Cloud Copilot to Act Security Labs

Many of the projects here began as part of **Cloud Copilot**.

Those projects are now moving to Act Security Labs, where they will continue to be developed as open-source software alongside new tools from the Act Security team.

If you've used or contributed to a Cloud Copilot project before: welcome to the new home.

---

## Use it wherever you build

Our goal is to make these tools useful without requiring you to adopt a particular platform or workflow.

Depending on the project, you can use them:

### In your terminal

Use the CLI directly, compose it into shell scripts, or add it to your existing automation.

### In your code

Use the underlying libraries to build IAM and cloud-security capabilities into your own applications.

### In your pipelines

Test policies and access changes as part of CI/CD before they reach production.

### In your browser

Many of our IAM tools are also available through **Amphi**, Act's free collection of cloud access tools.

---

## Build with us

These projects are built for practitioners, and we want practitioners involved in building them.

If you find a bug, have an idea, encounter an authorization edge case we haven't considered, or want to improve a tool:

- Open an issue
- Start a discussion
- Send a pull request
- Share a real-world use case

Cloud IAM has more than enough weird edge cases to go around.

---

## Security

If you believe you've discovered a security vulnerability in one of our projects, please follow the security reporting instructions in the repository rather than opening a public issue.

---

## About Act Security

[Act Security](https://act.security/) helps organizations control cloud access at the foundation.

Act models how identity, network, and AI access combine across cloud environments, helping security teams understand effective reachability, eliminate unnecessary access, and safely enforce stronger boundaries.

**Act Security Labs** is where we build in the open.
