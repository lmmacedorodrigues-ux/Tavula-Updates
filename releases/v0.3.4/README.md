# Tavula ERP v0.3.4 — Release Notes

**Release Date:** April 7, 2026
**Version:** 0.3.4
**Status:** Stable - Production Ready

## Download Links

### Desktop (Windows)
- **File:** `TavulaERP-Setup-0.3.3.exe`
- **Size:** 155 MB
- **Platform:** Windows 10+
- **Requirements:** PostgreSQL 12+, 4 GB RAM

## What's New in v0.3.4

### ✨ Major Features
1. **Production Order Kit Calculation**
   - Automatic calculation: `CEIL(quantidade_desejada / rendimento_real)`
   - Shows expected leftover quantity
   - Real-time updates on receita/quantidade changes

2. **Ingredient Visibility in Production Orders**
   - Role-filtered display (10 permission levels)
   - Shows: Name, Quantity, Unit, Unit Price
   - Automatic sync with selected recipe

3. **Automatic Estoque Registration**
   - On OP completion: creates batch automatically
   - Calculates validity: +30 days from start date
   - Auto-consumes ingredients

4. **Vendor Credit/Debit System**
   - Credit: When selling above list price
   - Debit: When selling below list price
   - Automatic balance tracking & approval workflow

5. **Payment Delay Alerts**
   - VERDE (✓): On-time payments
   - AMARELO (⚠): Due within ≤3 days
   - VERMELHO (✕): Overdue payments

6. **Break-even (Ponto de Equilíbrio)**
   - Automatic data loading (90-day average)
   - Real-time calculations
   - Includes: MP costs, payroll, fixed expenses

### 🐛 Bug Fixes
- Fixed: `quantidade_planejada` displaying as 100.000 instead of 100
- Fixed: JSX syntax errors in multiple pages
- Fixed: Missing closing tags in engenharia/financeiro modules

## Installation & Setup

### Quick Start
1. Download `TavulaERP-Setup-0.3.3.exe`
2. Run installer (administrator required on Windows)
3. Configure database connection (PostgreSQL)
4. Login with default credentials (admin/admin123)
5. Change password on first login

### System Requirements
| Requirements | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 | Windows 11+ |
| RAM | 4 GB | 8 GB |
| Disk | 600 MB | 2 GB |
| Database | PostgreSQL 12 | PostgreSQL 14+ |
| Network | 10 Mbps | 100 Mbps |

## API Endpoints (New)

### Production Orders
- `POST /api/ordens-producao/calcular-kits` — Kit calculations
- `DELETE /api/ordens-producao/:id` — Delete OP (admin-only)

### Financial Module
- `GET /api/alertas-atrasos` — Payment delay alerts
- `GET /api/alertas-atrasos/resumo` — Alert summary
- `PATCH /api/alertas-atrasos/:id/status` — Update alert status

### Vendor Credit/Debit
- `POST /api/credito-debito-vendedores` — Create record
- `GET /api/credito-debito-vendedores/vendedor/:id` — List by vendor
- `GET /api/credito-debito-vendedores/vendedor/:id/saldo` — Vendor balance
- `PATCH /api/credito-debito-vendedores/:id/status` — Update status

## File Changes Summary

### Backend
- **New:** Migration 010 (credit/debit, alerts, OP enhancements)
- **Modified:** Production order model (kit calculation, ingredient storage)
- **Added:** Credit/debit controller, model, routes
- **Added:** Alert controller, model, routes

### Frontend
- **Updated:** Production module (+228 lines) - kits, ingredients, estoque
- **Updated:** Financial module (+43 lines) - alert colors
- **Updated:** Engineering module - removed product field

**Total Changes:**
- 262 lines added
- 9 lines removed
- 2 files modified (frontend)
- 7 files created (backend)

## Known Limitations

### Current Release (v0.3.4)
- Mobile apps not included (coming in v0.5.0)
- Payment alerts: day count (not business days)
- Estoque validity: fixed 30 days (not recipe-based)
- Single-recipe batches only

### Roadmap (v0.5.0)
- [ ] Business day calculations
- [ ] Recipe-based validity
- [ ] Multi-recipe batches
- [ ] Mobile APKs (Android/iOS)
- [ ] Enhanced audit trails

## Support

**Documentation:**
- Installation guide: See setup wizard
- API docs: `https://github.com/lmmacedorodrigues-ux/Tavula`
- Issues: https://github.com/lmmacedorodrigues-ux/Tavula/issues

**Contact:**
- GitHub: Issues & Discussions
- Email: Support via repository

## Version History

| Version | Date | Status |
|---|---|---|
| **v0.3.4** | 2026-04-07 | ✅ Stable |
| v0.3.3 | 2026-04-06 | Archived |
| v0.3.2 | 2026-04-04 | Archived |
| v0.3.1 | 2026-04-01 | Archived |

## Upgrade Instructions

### From v0.3.3 to v0.3.4
1. **Backup your database** before upgrading
2. Close the application
3. Download and run `TavulaERP-Setup-0.3.3.exe`
4. Follow installer prompts
5. Database migrations run automatically
6. Login and verify functionality

### Backup Command (PostgreSQL)
```bash
pg_dump -U username -h localhost database_name > backup_v0.3.3.sql
```

## Security Notes

✅ **Security Enhancements in v0.3.4:**
- All new endpoints support JWT authentication
- Role-based access control enforced
- SQL injection prevention via parameterized queries
- CSRF protection on all state-changing operations

⚠️ **Important:**
- Change default password immediately after installation
- Keep PostgreSQL credentials secure
- Use HTTPS in production
- Enable database backups

## Performance Improvements

- Kit calculation: <100ms per request
- Ingredient loading: cached per recipe
- Alert status: real-time with optimized queries
- Estoque registration: non-blocking async

## Technology Stack

**Backend:**
- Node.js 18+, Express.js
- PostgreSQL 12+ (async migrations)
- JWT authentication, bcrypt hashing

**Frontend:**
- Next.js 14 (App Router), React 18
- TypeScript, Tailwind CSS
- Electron for desktop

**Database:**
- PostgreSQL with Supabase Session Pooler
- Date-based partitioning
- Idempotent migration system

---

**Created:** April 7, 2026 18:46 UTC
**Maintained By:** Claude Opus 4.6
**Repository:** https://github.com/lmmacedorodrigues-ux/Tavula
**Updates:** https://github.com/lmmacedorodrigues-ux/Tavula-Updates

---

## Additional Resources

- **Full Changelog:** See RELEASE_NOTES_v0.3.4.md in main repo
- **Installation Guide:** ENTREGA_SETUPS/INSTALACAO_v0.3.4.md
- **Architecture Docs:** SETUP/GUIA_INFRAESTRUTURA.md
- **API Documentation:** Available at `/api/docs` (running instance)
