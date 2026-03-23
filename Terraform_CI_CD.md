# Terraform und CI/CD

## Trouble

### 1. SSH Verbindung war nicht möglich, da Port 22 nicht freigeben war

- `ssh` Kommunikationen finden immer über den Port `22` statt
- Firewall blockiert standardmäßig alle Ports
- Wir mussten den Port 22 freischalten, sodass wir uns per ssh verbinden konnten

### 2. Wir haben gar keinen SSH Schlüssel auf der VM hinterlegt

- Voraussetzung wir haben ein Key-Pair
- Für heute haben wir uns über die AWS-Console einen Key-Pair erstellt (EC2 --> Sidebar --> Key-Pair --> Key-Pair erstellen --> Privater Schlüssel wurde zum Download bereitgestellt)
