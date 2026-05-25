# PC Transfer Workstation Setup

Use this note when moving the projects to another PC. The GitHub code backup is handled by the backup branches, but the new PC still needs the right tools installed.

## Install These Programs

Run these in PowerShell on the new PC:

```powershell
winget install --id Git.Git -e
winget install --id GitHub.cli -e
winget install --id Microsoft.VisualStudioCode -e
winget install --id OpenJS.NodeJS.LTS -e
winget install --id Python.Python.3.11 -e
winget install --id Docker.DockerDesktop -e
```

Install `uv` for Python project management:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installing, restart PowerShell and check:

```powershell
git --version
gh --version
node --version
npm --version
py --version
uv --version
docker --version
code --version
```

## What Each Tool Is For

- Git and GitHub CLI: clone repos, fetch branches, push work, and authenticate with GitHub.
- VS Code: edit and run the projects.
- Node.js/npm: most web, app, and dashboard projects use `package.json` and `package-lock.json`.
- Python 3.11/pip/uv: `kalshi-scout` and `TRADING`.
- Docker Desktop: `Autobot` and `Vector`.

## Project Tool Map

Node/npm projects:

- `audiotuner-local` / `cueforge`
- `crypto-intelligence`
- `financial-audit-dashboard`
- `FIT-CHECK`
- `fiverr-sniper-ai`
- `inboxpilot-ai`
- `micro-skills-mobile`
- `northbound-operator-site`
- `panda-ops`
- `pandora-desktop`
- `revenue-forge`
- `rift-runners`
- `storage-flip-assistant`
- `Vector`
- `yardnow`

Python projects:

- `kalshi-scout`
- `TRADING`

Docker projects:

- `Autobot`
- `Vector`

## First Steps On The New PC

Authenticate GitHub:

```powershell
gh auth login
```

Clone the repos you need:

```powershell
git clone https://github.com/P4ND4907/cueforge.git
git clone https://github.com/P4ND4907/Autobot.git
git clone https://github.com/P4ND4907/inboxpilot-ai.git
git clone https://github.com/P4ND4907/kalshi-scout.git
git clone https://github.com/P4ND4907/northbound-operator-site.git
git clone https://github.com/P4ND4907/revenue-forge.git
git clone https://github.com/P4ND4907/TRADING.git
git clone https://github.com/P4ND4907/Vector.git
git clone https://github.com/P4ND4907/yardnow.git
```

Fetch backup branches after cloning:

```powershell
git fetch --all --prune
```

Useful backup branches created before the PC move:

- `cueforge`: `backup/local-wip-20260525-005027-audiotuner-local-portable`
- `Autobot`: `backup/local-wip-20260525-005027-autobot`
- `inboxpilot-ai`: `backup/local-wip-20260525-005027-inboxpilot-ai`
- `kalshi-scout`: `backup/local-wip-20260525-005027-kalshi-scout`
- `northbound-operator-site`: `backup/local-wip-20260525-005027-northbound-operator-site`
- `revenue-forge`: `backup/local-wip-20260525-005027-revenue-forge`
- `TRADING`: `backup/local-wip-20260525-005027-trading`
- `Vector`: `backup/local-wip-20260525-005027-vector-portable`
- `yardnow`: `backup/local-wip-20260525-005027-yardnow`

## Restore Dependencies

For Node/npm projects:

```powershell
npm ci
```

For Python projects:

```powershell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

For Docker projects:

```powershell
docker compose up --build
```

## Do Not Forget Private Local Files

These files were intentionally not uploaded to GitHub because they may contain private data:

- `kalshi-scout/.env`
- `kalshi-scout/kalshi.db`
- `kalshi-scout/test_kalshi.db`

Copy those privately if they are needed on the new PC.

## Workflow File Note

GitHub rejected direct pushes that modify `.github/workflows/*` because the current token does not have `workflow` scope. For `cueforge` and `Vector`, workflow-file contents were copied into:

```text
docs/local-backups/workflow-files/
```

Use those copies to restore workflow edits later from a GitHub session or token that has workflow permission.
