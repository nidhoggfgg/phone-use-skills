# Phone Use Skills

**English** | [简体中文](README.zh-CN.md)

Installable agent Skills for [Phone Use](https://github.com/nidhoggfgg/PhoneUse), an Android observation and control service. This repository contains only the Skills and their runtime files, so installation does not download the Android source or its Git history.

## Install

```sh
npx skills add nidhoggfgg/phone-use-skills --skill phone-use
```

Choose your AI client and installation scope. The host needs Node.js 22.20+, Git, and Python 3.10+. Run Phone Use on your Android phone and connect over a reachable local network; pairing requires approval on the phone.

Then ask your agent:

> Use $phone-use to connect to http://192.168.1.20:8443. Show me the verification code, wait for my approval on the phone, then inspect the current screen.

See [Skill instructions](phone-use/SKILL.md) and the [installation guide](https://github.com/nidhoggfgg/PhoneUse/blob/main/docs/integrations.md).

## Maintenance

The main repository includes this repository as its `skills/` Git submodule. The Python client and API references are maintained in the main repository; run `python tools/sync_skill.py` there after editing them. Commit and push changes in this repository first, then commit the updated submodule pointer in the main repository. See the [contribution guide](https://github.com/nidhoggfgg/PhoneUse/blob/main/CONTRIBUTING.md).

Licensed under the [MIT License](LICENSE).
