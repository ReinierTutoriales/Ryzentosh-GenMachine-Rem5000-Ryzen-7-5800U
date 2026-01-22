# Ryzentosh GenMachine Ren5000 (Ryzen 7 5800U) — macOS Big Sur → Sequoia

![GenMachine Ren5000](IMG/4.png)

<div align="center">

<a href="https://www.reiniertutoriales.com/isos-raw-macos/">
  <img alt="macOS" src="https://img.shields.io/badge/macOS-Big%20Sur%20%E2%86%92%20Sequoia-000000?style=for-the-badge&logo=apple&logoColor=white">
</a>
<a href="https://github.com/dortania/build-repo/releases/download/OpenCorePkg-58f57a3/OpenCore-1.0.0-RELEASE.zip">
  <img alt="OpenCore 1.0.0" src="https://img.shields.io/badge/OpenCore-1.0.0-1f6feb?style=for-the-badge&logo=opencore&logoColor=white">
</a>
<a href="#">
  <img alt="Ryzentosh" src="https://img.shields.io/badge/Ryzentosh-Rem5000%20(5800U)-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

<br/><br/>

<a href="https://youtube.com/c/ReinierTutoriales">
  <img alt="YouTube" src="https://img.shields.io/badge/YouTube-ReinierTutoriales-FF0000?style=for-the-badge&logo=youtube&logoColor=white">
</a>
<a href="https://t.me/ReinierTutoriales">
  <img alt="Telegram" src="https://img.shields.io/badge/Telegram-Canal-26A5E4?style=for-the-badge&logo=telegram&logoColor=white">
</a>
<a href="https://twitter.com/ReinierTutorial">
  <img alt="X" src="https://img.shields.io/badge/X-@ReinierTutorial-000000?style=for-the-badge&logo=x&logoColor=white">
</a>
<a href="https://www.facebook.com/ReinierTutoriales">
  <img alt="Facebook" src="https://img.shields.io/badge/Facebook-ReinierTutoriales-1877F2?style=for-the-badge&logo=facebook&logoColor=white">
</a>
<a href="https://www.instagram.com/reiniertutoriales/">
  <img alt="Instagram" src="https://img.shields.io/badge/Instagram-@reiniertutoriales-E4405F?style=for-the-badge&logo=instagram&logoColor=white">
</a>
<a href="https://discord.gg/pQcCDBMn">
  <img alt="Discord" src="https://img.shields.io/badge/Discord-Comunidad-5865F2?style=for-the-badge&logo=discord&logoColor=white">
</a>

<br/><br/>

<a href="https://www.paypal.com/paypalme/ReinierTutoriales">
  <img alt="PayPal" src="https://img.shields.io/badge/PayPal-Donar-003087?style=for-the-badge&logo=paypal&logoColor=white">
</a>
<a href="https://www.patreon.com/ReinierTutoriales">
  <img alt="Patreon" src="https://img.shields.io/badge/Patreon-Apoyar-F96854?style=for-the-badge&logo=patreon&logoColor=white">
</a>
<a href="https://www.buymeacoffee.com/reiniertutoriales">
  <img alt="Café" src="https://img.shields.io/badge/Caf%C3%A9-Inv%C3%ADtame%20un%20caf%C3%A9-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black">
</a>

</div>

---

## Acerca de

EFI/guía para **GenMachine Ren5000** con **AMD Ryzen 7 5800U** orientada a ejecutar macOS en un entorno Ryzentosh. Incluye capturas de rendimiento y una base de configuración BIOS para reducir problemas comunes.

> Nota: En Ryzen, la compatibilidad depende fuertemente de versión de macOS, kexts y configuración. Ajusta tu EFI a tu hardware exacto.

---

## Estado / Compatibilidad

- **macOS:** Big Sur, Monterey, Ventura, Sonoma, Sequoia
- **Ryzentosh 2024**
- **OpenCore:** 1.0.0 (link de referencia arriba)

---

## Capturas

### macOS Ventura
![macOS Ventura](IMG/1.png)

---

## Rendimiento

### Geekbench 6 — macOS Ventura
![Geekbench 6](IMG/2.png)
![Geekbench 6](IMG/3.png)

---

## Especificaciones

| Componente   | Modelo |
|--------------|--------|
| CPU          | AMD Ryzen 7 5800U |
| Mini PC      | GenMachine Ren5000 |
| Memoria RAM  | 32GB DDR4 3200MHz |
| Gráficos     | AMD Radeon™ Graphics |
| Disco        | Western Digital 1TB WD Blue SN550 NVMe |
| Ethernet     | RealtekRTL8111 |
| BT/Wi-Fi     | Fenvi BCM94360NG |

---

## Configuración del BIOS

Aplica estos cambios (nombres pueden variar según BIOS/versión):

- **Advanced** → **Trusted Computing** → **Security Device Support** → **Disable**
- **AMD CBS** → **NBIO Common Options** → **IOMMU** → **Disabled**
- **GFX Configuration** → **IGPU Configuration** → **UMA Specified**
- **UMA Frame Buffer Size** → **16G**
- **Security** → **Secure Boot** → **Disabled**
- **Secure Boot Mode** → **Custom**
- **Boot** → **Quiet Boot** → **Disabled**
- **Boot** → **Fast Boot** → **Disabled**

---

## Recursos

- ISOs/RAW macOS (referencia): https://www.reiniertutoriales.com/isos-raw-macos/
- OpenCore 1.0.0 (build repo): https://github.com/dortania/build-repo/releases/download/OpenCorePkg-58f57a3/OpenCore-1.0.0-RELEASE.zip
