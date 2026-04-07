# Tavula ERP v0.3.4 — File Verification

## Desktop Installer: TavulaERP-Setup-0.3.3.exe

**File Size:** 155 MB (162,594,784 bytes)
**Release Date:** April 7, 2026
**Platform:** Windows 10 or higher

### Checksums for Verification

#### SHA256
```
06b0decf3bc4306d54efb473e8601118434a119c0ac516d4a590fc38fc3f7481
```

#### MD5
```
1753703924674ed07588a6c508b2686e
```

### How to Verify (Windows PowerShell)

#### Using SHA256 (recommended)
```powershell
cd "C:\path\to\downloaded\file"
$(Get-FileHash TavulaERP-Setup-0.3.3.exe -Algorithm SHA256).Hash
# Should output: 06b0decf3bc4306d54efb473e8601118434a119c0ac516d4a590fc38fc3f7481
```

#### Using MD5
```powershell
cd "C:\path\to\downloaded\file"
$(Get-FileHash TavulaERP-Setup-0.3.3.exe -Algorithm MD5).Hash
# Should output: 1753703924674ed07588a6c508b2686e
```

### How to Verify (Linux/macOS)

#### Using SHA256
```bash
sha256sum TavulaERP-Setup-0.3.3.exe
# Should output: 06b0decf3bc4306d54efb473e8601118434a119c0ac516d4a590fc38fc3f7481
```

#### Using MD5
```bash
md5sum TavulaERP-Setup-0.3.3.exe
# Should output: 1753703924674ed07588a6c508b2686e
```

### Installation Requirements

- **OS:** Windows 10 or higher
- **RAM:** Minimum 4 GB (8 GB recommended)
- **Disk Space:** 2 GB for installation + database
- **Database:** PostgreSQL 12+ (Supabase compatible)
- **Network:** Internet for initial setup and updates

### Integrity Check Recommended?

✅ **Yes!** Always verify file checksums before installation for security:
1. File may have been modified during download
2. Protects against man-in-the-middle attacks
3. Ensures you're installing an authentic Tavula release

### Still Have Issues?

If the checksum doesn't match:
1. Download the file again (different mirror/connection)
2. Clear browser cache
3. Check your download completed fully
4. Report to: https://github.com/lmmacedorodrigues-ux/Tavula/issues

---

**Generated:** April 7, 2026
**Format:** SHA256 + MD5 (for compatibility)
