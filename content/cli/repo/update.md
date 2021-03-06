---
title: "Update"
linkTitle: "Update"
description: >
  Learn how to modify a repo.
---

## Command

```
$ vela update repo <parameters...> <arguments...>
```

{{% alert color="info" %}}
For more information, you can run `vela update repo --help`.
{{% /alert %}}

## Parameters

The following parameters are used to configure the command:

| Name      | Description                  | Environment    |
| --------- | ---------------------------- | -------------- |
| `org`     | name of organization         | `REPO_ORG`     |
| `repo`    | name of repository           | `REPO_NAME`    |
| `link`    | full URL to repository       | `REPO_LINK`    |
| `clone`   | clone URL to repository      | `REPO_CLONE`   |
| `timeout` | max time allowed per build   | `REPO_TIMEOUT` |
| `private` | makes the repository private | `REPO_PRIVATE` |
| `trusted` | makes the repository trusted | `REPO_TRUSTED` |
| `event`   | events to trigger repository | `REPO_EVENT`   |
| `output`  | format the output            | `N/A`          |

{{% alert color="info" %}}
This command also supports setting the following parameters via a configuration file:

- `org`
- `repo`

For more information, please review the [CLI config documentation](/docs/cli/config/).
{{% /alert %}}

## Permissions

COMING SOON!

## Sample

{{% alert color="warning" %}}
This section assumes you have already installed and setup the CLI.

To install the CLI, please review the [installation documentation](/docs/cli/install/).

To setup the CLI, please review the [authentication documentation](/docs/cli/authentication/).
{{% /alert %}}

#### Request

```sh
vela update repo --org github --repo octocat --event tag
```

#### Response

```sh
repo "github/octocat" was updated
```
