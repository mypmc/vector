---
title: Environment Variables
sidebar_label: Env Vars
description: Vector's environment variables
---

<!--
     THIS FILE IS AUTOGENERATED!

     To make changes please edit the template located at:

     website/docs/reference/env-vars.md.erb
-->

You can control Vector's behavior through select environment variables:

```bash
ENV_VAR1=val ENV_VAR2=val vector --config=/etc/vector/vector.toml
```

In addition, we recommend that you look at the [global configuration 
options][docs.global-options] as well.

## Variables

import Fields from '@site/src/components/Fields';

import Field from '@site/src/components/Field';

<Fields filters={true}>


<Field
  enumValues={null}
  examples={["AKIAIOSFODNN7EXAMPLE"]}
  name={"AWS_ACCESS_KEY_ID"}
  path={null}
  required={false}
  type={"string"}
  >

### AWS_ACCESS_KEY_ID

Used for AWS authentication when communicating with AWS services. See relevant [AWS components][pages.aws_components] for more info.


</Field>


<Field
  enumValues={null}
  examples={["wJalrXUtnFEMI/K7MDENG"]}
  name={"AWS_SECRET_ACCESS_KEY"}
  path={null}
  required={false}
  type={"string"}
  >

### AWS_SECRET_ACCESS_KEY

Used for AWS authentication when communicating with AWS services. See relevant [AWS components][pages.aws_components] for more info.


</Field>


<Field
  enumValues={null}
  examples={["debug"]}
  name={"LOG"}
  path={null}
  required={false}
  type={"string"}
  >

### LOG

Sets Vector's log level. See the [log section in the monitoring guide][docs.monitoring#level] for more information on the available levels.


</Field>


<Field
  enumValues={null}
  examples={["debug"]}
  name={"RUST_BACKTRACE"}
  path={null}
  required={false}
  type={"string"}
  >

### RUST_BACKTRACE

Enables backtraces when errors are logged. Use this when debugging only since it can degrade performance.


</Field>


</Fields>


[docs.global-options]: /docs/reference/global-options
[docs.monitoring#level]: /docs/administration/monitoring#level
[pages.aws_components]: /components?providers%5B%5D=aws