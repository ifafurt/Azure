# 🚀 Azure Virtual Machine & File Share - Opdrachtverslag

**👤 Student:** Faruk  
**📅 Datum:** 23 november 2025  
**🎯 Doel:** Een virtuele machine opzetten en beheren via Microsoft Azure, inclusief bestandsdeling via Azure File Share.

---

## 1️⃣ Azure-account aanmaken

Ik heb een gratis proefaccount aangemaakt op Microsoft Azure en gebruikgemaakt van studentvoordelen om kosten te beperken en toegang te krijgen tot extra resources.

---

## 2️⃣ Resourcegroep aanmaken

Via de Azure Portal heb ik een nieuwe resourcegroep aangemaakt met de naam `farukRG`. De locatie is ingesteld op **West Europe (Zone 1)**.

<img width="1919" height="1079" alt="1" src="https://github.com/user-attachments/assets/1009e432-a46c-4d75-9f08-2f81b7f1d47e" />

---

## 3️⃣ Virtuele machine configureren

Ik heb een virtuele machine aangemaakt met de volgende instellingen:

- **Naam:** vit9  
- **Besturingssysteem:** Windows Server 2025 Datacenter Azure Edition  
- **Grootte:** Standard B2s (2 vCPU, 4 GiB RAM)  
- **Publiek IP-adres:** 4.231.122.66  
- **Netwerk:** vnet-westeurope/snet-westeurope-1  
- **Aangemaakt op:** 23 november 2025, 12:22 UTC

---

## 4️⃣ Verbinden met de VM

Via de Azure Portal heb ik een RDP-bestand gedownload en verbinding gemaakt met de VM. De desktopomgeving bevestigt een succesvolle verbinding.

<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/ea797273-061e-4da0-bfdb-acc5b5c6711f" />


---

## 5️⃣ Azure File Share aanmaken en koppelen

Ik heb een nieuwe **Storage Account** aangemaakt en daarin een **File Share** geconfigureerd met de naam `vi9dosyapayalas`. Deze heb ik gekoppeld aan zowel mijn VM als mijn lokale pc:

- **Windows:** Netwerkschijf gemapt als Z:  
- **Netwerkpad:** `\\vi19.file.core.windows.net\vi9dosyapayalas`

<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/6a7420b8-aa3d-4f5f-810e-620d0a219cab" />

---

## 6️⃣ Taken uitgevoerd op de VM

- **IIS-installatie:** IIS-webserver geïnstalleerd en standaard welkomstpagina gepubliceerd.  
- **SQL Server Express:** Verbonden via SSMS met `localhost\SQLEXPRESS` en databasebeheer geconfigureerd.

<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/3931973b-595a-42a2-a05e-afa3c9c6ce3d" />

<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/c7c00676-f7aa-4672-8ce7-949f431012af" />

---

## 7️⃣ Problemen en oplossingen

- ❌ **RDP-verbinding mislukt:** Poort 3389 was niet open in de Network Security Group.  
  ✅ Oplossing: NSG-regels aangepast om RDP-verkeer toe te staan.

---

## 8️⃣ Opruimen van resources

Na afronding van de opdracht heb ik alle resources verwijderd (VM, resourcegroep, storage account) om extra kosten te voorkomen.

---

> 📌 Deze opdracht bood een praktische introductie tot het werken met virtuele machines en bestandsdeling in Azure. Screenshots en configuraties zijn opgenomen ter ondersteuning van het leerproces.
