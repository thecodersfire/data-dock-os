# Built-in features for data-dock-os

Purpose: database development

1. **prepare a technical project** — run data-dock-os-workspace. It creates ~/Documents/data-dock-os-workspace/ with Design, Builds, Logs folders.
2. **plan a build or maintenance session** — run data-dock-os-plan to open a purpose-specific Markdown plan, saved under ~/Documents/data-dock-os-session-plans/.
3. **check technical change readiness** — run data-dock-os-check for an interactive checklist. Answers are not saved or transmitted.

These local tools create folders, open a local note, or display prompts. They do not install packages, change system settings, or send data.

Install them from this repository:

    mkdir -p "$HOME/.local/bin"
    install -m 0755 features/data-dock-os-workspace features/data-dock-os-plan features/data-dock-os-check "$HOME/.local/bin/"

## Preinstalled purpose software

The installer adds these three Flathub applications for database development:

1. **DB Browser for SQLite** — org.sqlitebrowser.sqlitebrowser
2. **GNOME Builder** — org.gnome.Builder
3. **Wireshark** — org.wireshark.Wireshark

They are installed from Flathub during setup. The repository contains application IDs and documentation, not third-party binaries; each publisher’s terms and licenses apply.
