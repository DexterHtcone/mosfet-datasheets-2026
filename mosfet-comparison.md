# Полный диалог и сравнение MOSFET-транзисторов

**Дата обновления:** 08.08.2026  
**Репозиторий:** https://github.com/DexterHtcone/mosfet-datasheets-2026

## Рабочие ссылки на даташиты (PDF)

### Высоковольтные
- **SPP20N60C3**: [Google Drive](https://drive.google.com/file/d/1YA8WgEpEe8SkwS6Zfq3MzhlQf_KceFl0/view?usp=drivesdk) | [Альтернатива](https://images.100y.com.tw/pdf_file/31-INFINEON-SPP20N60C3.pdf)
- **CRJT99N65G2**: данные через LCSC (оригинал 404)
- **JCS20N65FH**: через alltransistors.com
- **NCE65TF099**: [Google Drive](https://drive.google.com/file/d/1CZE7g00k0hZf8JyedDcgPfwsF392qySP/view?usp=drivesdk)

### Низковольтные
- **AONR62818**: [Google Drive](https://drive.google.com/file/d/1nZB6JwpgTR94B9wa0QQlprWSLkSxY1Lu/view?usp=drivesdk)
- **CSD19503KCS**: [Google Drive](https://drive.google.com/file/d/14_4TvO3lkmxnRAcEFF6yugPLUbLF12R5/view?usp=drivesdk) | [TI](https://www.ti.com/lit/gpn/CSD19503KCS)
- **AON6226**: [Google Drive](https://drive.google.com/file/d/1L4THwqYTHxYcsFs4DERg0ZzVSDEZi3jN/view?usp=drivesdk)
- **CRSM038N10N4**: данные через LCSC (оригинал 404)

---

## ⚡ Таблица 1: Высоковольтные MOSFET (650 В)

| Параметр                  | **SPP20N60C3**          | **CRJT99N65G2**       | **JCS20N65FH**          | **NCE65TF099**       |
|---------------------------|-------------------------|-----------------------|-------------------------|----------------------|
| **Производитель**         | Infineon               | CRMICRO              | Jilin Sino-Micro       | NCE Power           |
| **Технология**            | CoolMOS™ C3            | Super Junction       | Планарная              | Super Junction      |
| **Корпус**                | TO-220                 | TO-220               | TO-220F (изолир.)      | TO-220              |
| **VDS, В**                | 600 (650 Tjmax)        | 650                  | 650                    | 650                 |
| **ID (max), А**           | 20.7                   | 32–35                | 20                     | **38**              |
| **RDS(on) @ 25°C, мОм**   | 190                    | 81                   | 500                    | 89                  |
| **RDS(on) @ 100°C, мОм**  | ~240*                  | ~120*                | ~750*                  | ~135*               |
| **RthJC, °C/Вт**          | **0.6**                | **0.35**             | **~2.0–3.5** (изолир.) | **0.29**            |
| **Ciss (входная), нФ**    | ~2.4                   | 2.345                | ~4.0                   | 2.8                 |
| **Coss (выходная), пФ**   | ~780 (typ)             | 133                  | 250                    | ~97                 |
| **Crss (проходная), пФ**  | не указано             | 43                   | 11                     | ~1.5                |
| **Qg (затвор), нКл**      | **87**                 | 70                   | ~45–80                 | **45**              |
| **Pd (мощность), Вт**     | 208                    | 252                  | 62.2                   | 322                 |
| **Vgs(th), В**            | 2.1–3.9                | ~4.0                 | 5.0                    | 3.5                 |

> * – оценка ≈1.5×. RthJC для JCS — типичное для изолированных TO-220F.

---

## 🔋 Таблица 2: Низковольтные MOSFET (80–100 В)

| Параметр                  | **AONR62818**             | **CSD19503KCS**     | **AON6226**            | **CRSM038N10N4**     |
|---------------------------|---------------------------|---------------------|------------------------|----------------------|
| **Производитель**         | Alpha & Omega (AOS)      | Texas Instruments  | Alpha & Omega (AOS)   | CRMICRO             |
| **Технология**            | AlphaSGT™                | NexFET™            | AlphaSGT™             | SkyMOS4             |
| **Корпус**                | DFN-8 (3.3×3.3)          | TO-220             | DFN-8 (5×6)           | DFN-8 (5×6)         |
| **VDS, В**                | 80                       | 80                 | 100                   | 100                 |
| **ID (max), А**           | 50                       | **100**            | 48                    | **100**             |
| **RDS(on) @ 25°C, мОм**   | 6.6                      | 7.6                | 7.9                   | **3.2–3.6**         |
| **RDS(on) @ 100°C, мОм**  | ~9.9*                    | ~11.4*             | ~11.8*                | ~5.4                |
| **RthJC, °C/Вт**          | **~0.8–1.2** (через pad) | **0.8**            | **0.9–1.15**          | **0.5–0.9**         |
| **Ciss (входная), нФ**    | 2.42                     | не указано         | 3.13                  | 4.743               |
| **Coss (выходная), пФ**   | 280                      | не указано         | 245                   | 1025                |
| **Crss (проходная), пФ**  | **15**                   | Qgd = 5.4 нКл      | 12.5                  | ~80                 |
| **Qg (затвор), нКл**      | 48                       | **28**             | 60                    | 74.4                |
| **Pd (мощность), Вт**     | 54                       | 188                | 108                   | 139                 |
| **Vgs(th), В**            | 1.3–2.3                  | 2.8                | 1.3–2.3               | 3.0–3.8             |

> * – оценка ×1.5. Для SMD RthJC зависит от разводки платы.

---

## Ключевые выводы

- **Потери проводимости (HV)**: CRJT99N65G2 / NCE65TF099
- **Потери переключения**: NCE65TF099 (HV), CSD19503KCS (LV)
- **Теплоотвод**: лучшие CRJT (0.35) и NCE (0.29)

*Файл обновлён 08.08.2026*
