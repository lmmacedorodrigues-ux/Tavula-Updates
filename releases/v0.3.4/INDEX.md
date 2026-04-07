# Tavula ERP v0.3.4 Release — Complete Index

**Release Date:** April 7, 2026
**Status:** ✅ Production Ready
**Version:** 0.4.0 (Stable)

---

## 📥 Download Files

### Desktop Installer
**File:** `desktop/TavulaERP-Setup-0.3.3.exe`
- **Size:** 155 MB
- **Platform:** Windows 10+
- **Status:** Ready for Download
- **SHA256:** `06b0decf3bc4306d54efb473e8601118434a119c0ac516d4a590fc38fc3f7481`
- **MD5:** `1753703924674ed07588a6c508b2686e`

### Quick Download Link
Direct link (when on GitHub releases):
```
https://github.com/lmmacedorodrigues-ux/Tavula-Updates/releases/download/v0.3.4/TavulaERP-Setup-0.3.3.exe
```

---

## 📚 Documentation Files (This Directory)

### 1. **README.md** (START HERE)
- Overview of v0.3.4 features
- System requirements table
- Installation quick-start
- API endpoints list
- File changes summary
- Known limitations
- **Purpose:** Quick reference guide
- **Audience:** End users and developers

### 2. **RELEASE_ANNOUNCEMENT.md** (ANNOUNCEMENT)
- Official v0.3.4 announcement
- Download links with checksums
- Comprehensive feature descriptions
- Installation steps (5 minutes)
- Module features overview
- Performance metrics
- Technology stack
- Support and feedback channels
- **Purpose:** Public release announcement
- **Audience:** All stakeholders

### 3. **DELIVERY_SUMMARY.md** (COMPREHENSIVE)
- Complete implementation details
- All 6 features fully explained
- 18 API endpoints documented
- Database schema changes
- Bug fixes and improvements
- Security features detailed
- Testing checklist (13/13 passed)
- Implementation statistics
- v0.5.0 roadmap
- **Purpose:** Complete technical documentation
- **Audience:** Developers and technical team

### 4. **CHECKSUMS.md** (VERIFICATION)
- File integrity verification
- SHA256 and MD5 checksums
- How to verify on Windows/Linux/macOS
- Why verify your download
- Troubleshooting if checksum fails
- **Purpose:** Security and integrity validation
- **Audience:** Security-conscious users

### 5. **desktop/SHA256SUMS** (HASH FILE)
- Raw SHA256 checksum
- Location: `desktop/SHA256SUMS`
- Linux/macOS compatible format
- **Use:** `sha256sum -c SHA256SUMS`

### 6. **desktop/MD5SUMS** (HASH FILE)
- Raw MD5 checksum
- Location: `desktop/MD5SUMS`
- For additional verification
- Note: Consider SHA256 preferred over MD5

---

## 📖 Related Documentation (Main Repository)

### In Main Repository (lmmacedorodrigues-ux/Tavula)

**SETUP/ Directory:**
```
SETUP/atualizacoes/CHANGELOG.md
  → Complete version history (v0.1.6 through v0.3.4)
  → All changes and improvements documented

SETUP/INSTALACAO_v0.3.4.md (OR ENTREGA_SETUPS/)
  → Detailed installation guide for v0.3.4
  → Troubleshooting and common issues
  → System requirements verification

SETUP/GUIA_INFRAESTRUTURA.md
  → Infrastructure setup guide
  → Database configuration
  → Deployment options
  → VPS and cloud setup

SETUP/RELEASE_NOTES_v0.3.4.md
  → Official release notes
  → Feature descriptions
  → Bug fixes documented
  → Known limitations
```

**API Documentation:**
```
Available at: /api/docs (when Tavula is running)
  → Interactive API documentation
  → Endpoint testing interface
  → Request/response examples
```

---

## 🎯 Quick Start (Choose Your Path)

### For End Users
1. Read: `README.md` (this directory)
2. Download: `desktop/TavulaERP-Setup-0.3.3.exe`
3. Verify: Use `CHECKSUMS.md`
4. Install: Follow steps in `RELEASE_ANNOUNCEMENT.md`
5. Learn: Read main repository's `INSTALACAO_v0.3.4.md`

### For Developers / IT Admins
1. Read: `DELIVERY_SUMMARY.md` (comprehensive)
2. Review: `RELEASE_NOTES_v0.3.4.md` (main repo)
3. Setup: Follow `GUIA_INFRAESTRUTURA.md` (main repo)
4. Deploy: Configure database and run installer
5. Test: Verify against testing checklist
6. Integrate: Use API endpoints from documentation

### For IT Security / Compliance
1. Read: Security section in `DELIVERY_SUMMARY.md`
2. Review: Checksum verification in `CHECKSUMS.md`
3. Verify: File integrity before deployment
4. Audit: Access logs and database changes
5. Backup: Before installation and regularly after

---

## 📊 What Changed in v0.3.4

### Major Features (6 Total)
✅ Production Order Kit Calculation
✅ Ingredient Visibility in Production Orders
✅ Automatic Estoque Registration
✅ Vendor Credit/Debit System
✅ Payment Delay Visual Alerts
✅ Break-even Analysis (Previously implemented)

### Code Changes
- **Lines Added:** 262
- **Lines Removed:** 9
- **Files Modified:** 2
- **Files Created:** 7
- **Migrations:** 1 new

### API Endpoints
- **New Endpoints:** 8
- **Total Available:** 18+
- **Authentication:** JWT on all new endpoints
- **Access Control:** Role-based (10 levels)

### Bug Fixes
- ✅ Quantity formatting (100 vs 100.000)
- ✅ JSX syntax errors (engenharia/financeiro)
- ✅ Missing HTML tags
- ✅ Form validation improvements

---

## 🔒 Security Highlights

✅ **Implemented:**
- JWT authentication
- Role-based access control
- SQL injection prevention
- CSRF protection
- Input validation
- Secure password hashing

⚠️ **Important:**
- Change default password after installation
- Keep credentials secure
- Use HTTPS in production
- Regular database backups
- Monitor access logs

---

## 📋 System Requirements

| Requirement | Minimum | Recommended |
|-------------|---------|------------|
| **OS** | Windows 10 | Windows 11+ |
| **RAM** | 4 GB | 8 GB |
| **Disk** | 2 GB | 4 GB+ |
| **Database** | PostgreSQL 12 | PostgreSQL 14+ |
| **Network** | 10 Mbps | 100 Mbps |
| **Node.js** | 18.x | 20.x LTS |

---

## ✅ Testing Status

All 13 items on testing checklist passed:
- [x] Kit calculation accuracy
- [x] Ingredient role filtering
- [x] Estoque auto-registration
- [x] Alert colors display correctly
- [x] Break-even calculations
- [x] Vendor balance tracking
- [x] Desktop installer build
- [x] TypeScript compilation
- [x] Production builds
- [x] Database migrations
- [x] JWT authentication
- [x] Role-based access control
- [x] All edge cases handled

---

## 🚫 Known Limitations

### v0.3.4
- Mobile apps not in desktop installer (separate APKs)
- Payment alerts: calendar days (not business days)
- Estoque validity: fixed 30 days (not recipe-specific)
- Kit calculation: uniform yield assumption

### v0.5.0 (Planned)
- [ ] Business day calculations
- [ ] Recipe-based validity
- [ ] Multi-recipe estoque support
- [ ] Mobile app distribution
- [ ] Enhanced audit trails
- [ ] Advanced reporting

---

## 🔗 Important Links

**GitHub Repositories:**
- Main: https://github.com/lmmacedorodrigues-ux/Tavula
- Updates: https://github.com/lmmacedorodrigues-ux/Tavula-Updates
- Issues: https://github.com/lmmacedorodrigues-ux/Tavula/issues

**Documentation:**
- Installation inside: `ENTREGA_SETUPS/INSTALACAO_v0.3.4.md`
- Release notes inside: `SETUP/atualizacoes/CHANGELOG.md`
- API docs: Available at `/api/docs` (running instance)

**Support:**
- Issues: GitHub Issues
- Discussions: GitHub Discussions
- Email: Via repository issues

---

## 📞 Support & Troubleshooting

### Common Questions

**Q: How do I install Tavula?**
A: Download the .exe file and run it. Administrator privileges required. Follows Windows installer standard practices.

**Q: What database do I need?**
A: PostgreSQL 12 or higher. Can use local or cloud (Supabase, Railway, etc.).

**Q: Can I use this in production?**
A: Yes! v0.3.4 is marked as production-ready and fully tested.

**Q: Are there mobile apps?**
A: Mobile apps are in development. Separate APK downloads will be available soon.

**Q: How do I update from v0.3.3?**
A: Install v0.3.4 over existing installation. Database migrations run automatically.

### Troubleshooting

**Database connection fails:**
1. Verify PostgreSQL is running
2. Check credentials
3. Verify network connectivity
4. Check firewall (port 5432)

**Login issues:**
1. Use default: `admin` / `admin123`
2. Verify database populated (migrations ran)
3. Check database logs

**Feature not visible:**
1. Verify user role has permission
2. Check module is available
3. Refresh browser/application
4. Verify database schema matches

---

## 🎓 Learning Resources

**Inside Desktop App:**
- Help tooltips on hover
- Module documentation in settings
- Sample data in test mode

**In Repository:**
- API documentation: `/api/docs`
- Code comments and docstrings
- Type definitions (.ts files)
- Database schema in migrations

**External:**
- GitHub Discussions for questions
- Issues for bug reports
- Wiki (if created)

---

## 📝 File Organization

```
releases/v0.3.4/
├── README.md                    (START: Overview)
├── RELEASE_ANNOUNCEMENT.md      (PUBLIC: Official announcement)
├── DELIVERY_SUMMARY.md          (DETAILED: Complete technical docs)
├── CHECKSUMS.md                 (SECURITY: File verification)
├── desktop/
│   ├── TavulaERP-Setup-0.3.3.exe   (→ Download this)
│   ├── SHA256SUMS               (→ Verify with this)
│   └── MD5SUMS                  (→ Alternative verification)
└── [This Index File]            (Navigation guide)
```

---

## 🏁 Next Steps

1. **Download** the installer
2. **Verify** using checksums (optional but recommended)
3. **Read** README.md or RELEASE_ANNOUNCEMENT.md
4. **Install** following setup wizard
5. **Configure** database connection
6. **Test** with sample data
7. **Deploy** to production
8. **Monitor** and report issues

---

## 📊 Release Statistics

**Files in This Release:**
- 1 Desktop installer (155 MB)
- 4 Documentation files (README, Announcement, Summary, Checksums)
- 2 Checksum verification files (SHA256, MD5)
- **Total:** 7 files

**Time to Download:** ~15 minutes at 10 Mbps (~1 minute at 100 Mbps)
**Time to Install:** ~2-3 minutes
**Time to Configure:** ~5 minutes
**Time to Begin Using:** <15 minutes total

---

**Release Prepared:** April 7, 2026
**Version:** 0.4.0 (Stable - Production Ready)
**Maintained By:** Claude Opus 4.6
**Repository:** https://github.com/lmmacedorodrigues-ux/Tavula
**Updates Repository:** https://github.com/lmmacedorodrigues-ux/Tavula-Updates

---

*Last Updated: April 7, 2026*
*Status: All files ready for production deployment*
