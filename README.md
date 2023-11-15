# Repo Scaffolder
Templates and commandline tools for creating repositories for US Federal open source projects

## Prerequisites
- python
- github cli
- cookiecutter

## Need help picking a tier?
If you do not know what tier you project is the cookiecutter will walk you through questions to figure out what tier you need.  Run:
```
cookiecutter https://github.com/DSACMS/repo-scaffolder
```

## Know what tier you need?
If you know what tier you need you can run the cookiecutter for an individual tier.  Use the below command with `X` substituted for the tier number.
```
cookiecutter https://github.com/DSACMS/repo-scaffolder --directory=tierX
```

## Existing Projects
You can update existing projects with the repo scaffolder.  Using the `-s` flag on cookiecutter will not overwrite existing files.  Follow these steps:
1. Create a new branch in your repo
2. cd into folder above
3. run: `cookiecutter -f -s https://github.com/DSACMS/repo-scaffolder --directory=tierX`
4. Make sure when answering the questions you use the existing folder/project name
5. Raise pr into main

## Updating Projects
When creating projects, if you want to receive updates then add `dsacms-tierX`
as a github topic to the repo.  The scaffolder repo includes github workflows
that will find all repos with that tag and can raise a pull request with an
updated string or adding a file.

## Maturity Models
See our Maturity Model Tiers Document for reference: https://github.com/DSACMS/repo-scaffolder/blob/main/maturity-model-tiers.pdf

## Acknowlegements
This project was developed as a collaboration between the United States Digital
Service ([USDS.gov](https://usds.gov)), The Department of Health and Human
Services ([HHS.gov](https://hhs.gov)), The Digital Service at the Centers for
Medicare & Medicaid Services ([CMS.gov](https://cms.gov)) and The
[USDigitalResponse.org](https://usdigitalresponse.org).

## Policies

### Open Source Policy

We adhere to the [CMS Open Source
Policy](https://github.com/CMSGov/cms-open-source-policy). If you have any
questions, just [shoot us an email](mailto:opensource@cms.hhs.gov).

### Security and Responsible Disclosure Policy

The Centers for Medicare & Medicaid Services is committed to ensuring the
security of the American public by protecting their information from
unwarranted disclosure. We want security researchers to feel comfortable
reporting vulnerabilities they have discovered so we can fix them and keep our
users safe. We developed our disclosure policy to reflect our values and uphold
our sense of responsibility to security researchers who share their expertise
with us in good faith.

*Submit a vulnerability:* Unfortunately, we cannot accept secure submissions via
email or via GitHub Issues. Please use our website to submit vulnerabilities at
[https://hhs.responsibledisclosure.com](https://hhs.responsibledisclosure.com).
HHS maintains an acknowledgements page to recognize your efforts on behalf of
the American public, but you are also welcome to submit anonymously.

Review the HHS Disclosure Policy and websites in scope:
[https://www.hhs.gov/vulnerability-disclosure-policy/index.html](https://www.hhs.gov/vulnerability-disclosure-policy/index.html).

This policy describes *what systems and types of research* are covered under this
policy, *how to send* us vulnerability reports, and *how long* we ask security
researchers to wait before publicly disclosing vulnerabilities.

If you have other cybersecurity related questions, please contact us at
[csirc@hhs.gov](mailto:csirc@hhs.gov).

## Public domain

This project is in the public domain within the United States, and copyright
and related rights in the work worldwide are waived through the [CC0 1.0
Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0 dedication. By
submitting a pull request or issue, you are agreeing to comply with this waiver
of copyright interest.
