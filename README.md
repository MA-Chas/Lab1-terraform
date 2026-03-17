# Lab 1 Terraform

## Vad gör projektet
Detta projekt använder Terraform för att automatisera skapandet av en virtuell maskin i Google Cloud. Konfigurationen bygger upp en Compute Engine‑instans, kör ett startup‑script och skapar en daglig backup‑policy. Projektet visar hur infrastruktur kan definieras som kod och köras både lokalt och via GitHub Actions.

# Köra lokalt

```bash
terraform init
terraform plan
terraform apply
```

## Screenshot-Pipeline
<img width="450" height="335" alt="Pipeline" src="https://github.com/user-attachments/assets/1dc57b22-daa1-47c5-8068-a8d6f01fe13e" />

## Screenshot-GCP VM
<img width="1412" height="700" alt="VM instances" src="https://github.com/user-attachments/assets/4127518f-f160-40f3-b902-d253752fe233" />


## Säkerhetsbeslut
- `ufw`: används för att begränsa inkommande trafik och endast tillåta nödvändiga portar.
- ` fail2ban`: skyddar mot brute‑force‑attacker genom att blockera IP‑adresser med upprepade felaktiga inloggningar. 
