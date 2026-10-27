# Data dictionary: `bank_data.csv`

Balanced annual panel: 7 banks x 12 years (2004-2015) = 84 rows. One row per bank-year.

**Sources (secondary data):** Central Bank of Kenya (CBK) Bank Supervision Annual Reports; the banks' published audited annual reports; Nairobi Securities Exchange (NSE) publications.

| Column | Description | Unit |
|---|---|---|
| `BANK` | Bank identifier: BARCLAYS, CFC_STANBIC, DTB, KCB, NBK, NIC, STANCHART | - |
| `YEAR` | Financial year | year |
| `ROAA` | Return on average assets (outcome variable) | % |
| `ROAE` | Return on average equity | % |
| `CAR_%` | Capital adequacy ratio | % |
| `LDR_%` | Loan-to-deposit ratio (advances / deposits) | % |
| `NPL_%` | Non-performing loans as a share of loans | % |
| `CIR_%` | Cost-to-income ratio | % |
| `SIZE_LN_ASSETS` | Natural log of net assets (KSh millions) | log |
| `NIM_%` | Net interest margin | % |
| `LIQUIDITY_%` | Liquidity ratio | % |
| `Net Assets (KSh M)` | Net assets | KSh millions |
| `Advances (KSh M)` | Loans and advances | KSh millions |
| `Deposits (KSh M)` | Customer deposits | KSh millions |

**Consistency checks (run in the notebook):** `LDR_%` reproduces from `Advances / Deposits` to within 0.05 percentage points, and `SIZE_LN_ASSETS` reproduces from `ln(Net Assets)` to within 0.00005. Figures were not re-verified line by line against the source reports.
