# Script ksdeps

[Version en español](./README.md)

This is a script that has the purpose of generating the kls-classpath file from a Kotlin script for kscript, using an unofficial function of the kscript command itself (`kscript --dependencies <script kotlin>`), which is proposed in this [PR](https://github.com/kscripting/kscript/pull/420).

## Execution

```bash
/path/to/script/ksdeps <script kotlin>
```

## Points to consider

This script collects the dependencies returned by kscript and adds both the kotlin stdlib as exemplified [here](https://github.com/fwcd/kotlin-language-server/tree/main?tab=readme-ov-file#figuring-out-the-dependencies) and metadata annotations for kscript, more information [here](https://github.com/kscripting/kscript?tab=readme-ov-file#script-configuration).
