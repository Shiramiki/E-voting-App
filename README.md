# E-voting-App


#File structure
## Repo root (unchanged):

E-voting-App/
├── e_voting_console_app.py   # Original monolith (do not modify; reference only)
├── Software_construction_Easter_Test_2026.pdf
├── README.md                 # Can stay minimal at root; full report lives in the new folder
└── refactored/               # All new work goes here
    └── ... (layout below)

## Inside the new folder (e.g. refactored/):

refactored/
├── README.md                 # Report: structure + design decisions (1–2 pages)
├── requirements.txt         # Optional; stdlib may suffice
├── e_voting_console_app.py   # Entry point (same name as original): load data, login loop, dispatch to dashboards
├── ui/
│   ├── __init__.py
│   ├── console.py            # Colors, header, subheader, table_*, error/success/warning/info, menu_item, prompt, masked_input, clear_screen, pause
│   └── themes.py             # THEME_* constants (optional)
├── models/
│   ├── __init__.py
│   ├── candidate.py
│   ├── station.py
│   ├── poll.py
│   ├── position.py
│   ├── voter.py
│   ├── admin.py
│   └── vote.py
├── services/
│   ├── __init__.py
│   ├── auth_service.py
│   ├── candidate_service.py
│   ├── station_service.py
│   ├── poll_service.py
│   ├── voter_service.py
│   ├── admin_service.py
│   ├── voting_service.py
│   └── audit_service.py
├── data/
│   ├── __init__.py
│   ├── store.py
│   └── repository.py         # Optional
└── app/
    ├── __init__.py
    ├── login_flow.py
    ├── admin_dashboard.py
    └── voter_dashboard.py
