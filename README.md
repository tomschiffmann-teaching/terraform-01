## 1. Umgebungsvariablen setzen

5
4

- Die Umgebuzngsvariablen sind Teil der Session im Terminal/Powershell
- Im AWS Kontext nutzen wir die Env-Variablen, um unseren `AWS_ACCESS_KEY_ID` und `AWS_SECRET_ACCESS_KEY` zu setzen

### Linux

`export AWS_ACCESS_KEY_ID=`

`export AWS_SECRET_ACCESS_KEY=`

`export AWS_DEFAULT_REGION=us-east-1`

### Windows

`$env:AWS_ACCESS_KEY_ID=""`
`$env:AWS_SECRET_ACCESS_KEY=""`
`$env:AWS_DEFAULT_REGION="us-east-1"`

## Terraform state

### Workflow

![Basic Workflow](./images/tfstate_workflow.png)

### TF State Remote in Speicher ablegen

![](./images/tfstate_solution.png)
