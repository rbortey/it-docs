# Remote Access Notes

Remote access profiles are issued for support windows and should be scoped to the business need.

## Profile Types

| Profile type | Route scope | Typical owner |
|---|---|---|
| Staff support | User LAN and approved services | IT support |
| Vendor limited | Single host or narrow segment | Service desk lead |
| Admin operations | Management systems | Infrastructure |

## Guidance

- Client-side route lists are convenience settings, not security controls.
- Server-side firewall policy must enforce the allowed destination scope.
- Each vendor profile should map to a unique peer address so activity can be tracked.
- Expired vendor profiles should be removed from active peer lists.

## Naming Convention

```text
wg-<department>-<supplier>-<purpose>-<yyyymm>.conf
```

Examples:

```text
wg-fin-recon-support-202407.conf
wg-ops-atm-maint-202407.conf
```