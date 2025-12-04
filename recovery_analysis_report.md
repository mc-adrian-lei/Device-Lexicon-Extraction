# Device Lexicon Analysis Report
## Samsung Galaxy A51 Recovery Boot Evidence

### Device Identification
- **Model**: SM-A515U1 (AT&T variant)
- **SoC**: Exynos 9611
- **Build**: TPIA.220624.014 (February 2024)
- **Bootloader**: A515U1UESCFXA2

### Security Posture
- ✓ Bootloader: LOCKED
- ✓ Partitions: LOCKED  
- ✓ Build Type: user (production)
- ✓ Build Tags: release-keys
- ✓ Security Patch: 2024-01-01

### Recovery Event Evidence
- **Action**: Factory Data Reset initiated
- **Wipe Data**: CONFIRMED
- **Wipe Cache**: CONFIRMED
- **Display**: 2400×1080 (S6E3 panel)
- **EFS Error**: Device or resource busy (normal during shutdown)

### Lexicon Summary
| Screen | Category | Properties | Components |
|--------|----------|-----------|------------|
| Image 1 | LMK Config | 13 | 0 |
| Image 2 | Filesystem | 0 | 1 |
| Image 3 | Init/Display | 0 | 8 |
| Image 5 | Sys/Vendor | 9 | 0 |
| Image 6 | HW/Setup | 9 | 0 |
| Image 7 | Dalvik VM | 8 | 0 |
| Image 8 | Boot Params | 9 | 2 |
| Image 9 | Build Info | 11 | 0 |
| Image 10 | Recovery UI | 0 | 9 |

**Total**: 59 properties, 20 components identified across 9 images

### Forensic Notes
- Device was in recovery mode during factory reset
- All security locks were engaged (production state)
- No evidence of bootloader unlocking or developer mode
- Standard Samsung recovery UI with system property dumps
- Images span multiple boot-time property lists and UI rendering stages
