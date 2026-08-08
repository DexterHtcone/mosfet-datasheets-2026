# Полный диалог и сравнение MOSFET-транзисторов

**Дата обновления:** 08.08.2026  
**Статус:** 8/8 даташитов  
**Репозиторий:** https://github.com/DexterHtcone/mosfet-datasheets-2026

## Все 8 ссылок на PDF

| Транзистор | PDF |
|------------|-----|
| **SPP20N60C3** | [Google Drive](https://drive.google.com/file/d/1YA8WgEpEe8SkwS6Zfq3MzhlQf_KceFl0/view?usp=drivesdk) |
| **CRJT99N65G2** | [Google Drive](https://drive.google.com/file/d/1w15fZcKksMPIjS3728R7aMaFtSzfr6Km/view?usp=drivesdk) |
| **JCS20N65FH** | [Google Drive](https://drive.google.com/file/d/1fiAWz1gEGtNDL5-XRSGXeqSDqMR9bjYQ/view?usp=drivesdk) |
| **NCE65TF099** | [Google Drive](https://drive.google.com/file/d/1CZE7g00k0hZf8JyedDcgPfwsF392qySP/view?usp=drivesdk) |
| **AONR62818** | [Google Drive](https://drive.google.com/file/d/1nZB6JwpgTR94B9wa0QQlprWSLkSxY1Lu/view?usp=drivesdk) |
| **CSD19503KCS** | [Google Drive](https://drive.google.com/file/d/14_4TvO3lkmxnRAcEFF6yugPLUbLF12R5/view?usp=drivesdk) |
| **AON6226** | [Google Drive](https://drive.google.com/file/d/1L4THwqYTHxYcsFs4DERg0ZzVSDEZi3jN/view?usp=drivesdk) |
| **CRSM038N10N4** | [Google Drive](https://drive.google.com/file/d/1b9idNC3gx4feR3dlbiDOZKk3Ja5CX7Qs/view?usp=drivesdk) |

---

## ⚡ Таблица 1: Высоковольтные MOSFET (650 В)

| Параметр | **SPP20N60C3** | **CRJT99N65G2** | **JCS20N65FH** | **NCE65TF099** |
|----------|---------------|-----------------|----------------|----------------|
| Производитель | Infineon | CRMICRO | Jilin Sino-Micro | NCE Power |
| Технология | CoolMOS C3 | Super Junction | Планарная | Super Junction |
| Корпус | TO-220 | TO-220 | **TO-220MF (изолир.)** | TO-220 |
| VDS | 600 (650 Tjmax) | 650 | 650 | 650 |
| ID max | 20.7 A | 32–35 A | 20 A | **38 A** |
| RDS(on) @25°C | 190 мОм | **81 мОм** | 500 мОм (typ 440) | 89 мОм |
| RDS(on) @100°C | ~240* | ~120* | ~750* | ~135* |
| **RthJC** | **0.6** | **0.35** | **2.01** | **0.29** |
| Ciss | ~2.4 нФ | 2.345 нФ | 2.55 нФ (typ) | 2.8 нФ |
| Coss | ~780 пФ | 133 пФ | 250 пФ | ~97 пФ |
| Crss | не указано | 43 пФ | **11 пФ** | ~1.5 пФ |
| Qg | **87 нКл** | 70 нКл | **45 нКл** (max 80) | **45 нКл** |
| Pd | 208 W | 252 W | 62.2 W | 322 W |
| Vgs(th) | 2.1–3.9 | ~4.0 | 3.0–5.0 | 3.5 |

> * – оценка ×1.5

## 🔋 Таблица 2: Низковольтные MOSFET (80–100 В)

| Параметр | **AONR62818** | **CSD19503KCS** | **AON6226** | **CRSM038N10N4** |
|----------|---------------|-----------------|-------------|------------------|
| Производитель | AOS | Texas Instruments | AOS | CRMICRO |
| Технология | AlphaSGT | NexFET | AlphaSGT | SkyMOS4 |
| Корпус | DFN 3.3×3.3 | TO-220 | DFN 5×6 | DFN 5×6 |
| VDS | 80 | 80 | 100 | 100 |
| ID max | 50 A | **100 A** | 48 A | **100 A** |
| RDS(on) @25°C | 6.6 мОм | 7.6 мОм | 7.9 мОм | **3.2–3.6 мОм** |
| RDS(on) @100°C | ~9.9* | ~11.4* | ~11.8* | ~5.4 |
| **RthJC** | ~0.8–1.2 | **0.8** | 0.9–1.15 | 0.5–0.9 |
| Ciss | 2.42 нФ | не указано | 3.13 нФ | 4.743 нФ |
| Coss | 280 пФ | не указано | 245 пФ | 1025 пФ |
| Crss | **15 пФ** | Qgd=5.4 нКл | 12.5 пФ | ~80 пФ |
| Qg | 48 нКл | **28 нКл** | 60 нКл | 74.4 нКл |
| Pd | 54 W | 188 W | 108 W | 139 W |
| Vgs(th) | 1.3–2.3 | 2.8 | 1.3–2.3 | 3.0–3.8 |

---

## Ключевые выводы (финал)

- **Лучшие по RDS(on) HV**: CRJT99N65G2 (81 мОм) и NCE65TF099 (89 мОм)
- **Лучшие по Qg HV**: NCE65TF099 и JCS20N65FH (оба 45 нКл)
- **Лучший тепловой контакт**: CRJT99N65G2 (RthJC = 0.35) и NCE65TF099 (0.29)
- **Изолированный корпус**: JCS20N65FH (RthJC = 2.01 °C/Вт) — удобно, но теплоотвод хуже
- **LV-лидер по проводимости**: CRSM038N10N4 (3.2–3.6 мОм)
- **LV-лидер по переключению**: CSD19503KCS (Qg = 28 нКл)

*Все данные проверены по оригинальным даташитам 08.08.2026*
