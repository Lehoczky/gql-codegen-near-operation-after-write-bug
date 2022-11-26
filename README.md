# GraphQL Code generator near operation file preset with hooks

## Repro Steps

Install the dependencies:

```console
npm i
```

Run the code generation:

```console
npm run codegen
```

The result:

```console
> graphql-code-generator

✔ Parse Configuration
✔ Generate outputs
Error: Command failed: prettier --write C\:/Users/ifjle/Projects/gql-codegen-near-operation-after-write-bug/src/query.generated.ts src/types.ts
[error] No files matching the pattern were found: "C\:/Users/ifjle/Projects/gql-codegen-near-operation-after-write-bug/src/query.generated.ts".

    at ChildProcess.exithandler (node:child_process:400:12)
    at ChildProcess.emit (node:events:513:28)
    at ChildProcess.emit (node:domain:489:12)
    at maybeClose (node:internal/child_process:1093:16)
    at Process.ChildProcess._handle.onexit (node:internal/child_process:302:5) {
  code: 2,
  killed: false,
  signal: null,
  cmd: 'prettier --write C\\:/Users/ifjle/Projects/gql-codegen-near-operation-after-write-bug/src/query.generated.ts src/types.ts'
}
```
