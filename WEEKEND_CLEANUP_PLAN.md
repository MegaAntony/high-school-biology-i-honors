# Weekend Directory Cleanup & Migration Guide
### Biology I Honors • Academic Year 2026–2027 • Grade 9
*Scheduled for Execution: **Friday Evening (9/11) or Saturday (9/12)***

---

## 🎯 Executive Summary & Purpose

Today (Friday 9/11) was Quiz Day on Unit 2 Part 1 (Cell Membrane & Transport). To protect live quiz access, the legacy environment was kept 100% frozen. 

Now that the master V2 repository ([`MegaAntony/high-school-biology-i-honors`](https://github.com/MegaAntony/high-school-biology-i-honors)) is fully deployed, validated (**281 valid links / 0 broken**), and live on GitHub Pages, the older redundant local directories on the Mac can be cleaned up over the weekend.

---

## 📁 Local Directories Audit & Disposition

| Directory Path | Current Status | Disposition | Action Plan |
| :--- | :--- | :--- | :--- |
| `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors-V2` | **Active Production** | **KEEP PERMANENTLY** | Primary workspace for the rest of the school year. |
| `/Volumes/Backup/Antony/HighSchool/Grade9/Biology` | Redundant Scratch (Aug 27) | **DELETE SAFELY** | 100% of files exist in V2. Not a git repository. |
| `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors` | Legacy Production (V1) | **DELETE LOCAL CLONE** | Remote GitHub repo remains intact; local folder no longer needed. |

---

## 🔍 Why It Is Safe to Delete the Legacy Folders

### 1. `/Volumes/Backup/Antony/HighSchool/Grade9/Biology`
* **What it was:** Early scratch folder from the beginning of Unit 1 (Biochemistry).
* **Data Safety:** An automated differential audit confirmed that **0 files are missing** from V2. All lecture notes, PDF packets, standards, and tests were cataloged into [`Biology-Honors-V2/units/unit-01-biochemistry/`](units/unit-01-biochemistry/).
* **Risk level:** **Zero Risk.**

### 2. `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors`
* **What it was:** The initial Git repository cloned for Unit 2 Part 1.
* **Remote GitHub Pages Remains Online:** Deleting the local directory on the Mac **DOES NOT delete or modify the remote GitHub repository** ([`MegaAntony/biology-honors`](https://github.com/MegaAntony/biology-honors)). The live website ([`https://megaantony.github.io/biology-honors/`](https://megaantony.github.io/biology-honors/)) and all existing bookmarks will remain live on GitHub's servers indefinitely.
* **100% Preserved in V2:** All 26 tests, the 55-question master test, the 1-column cheat sheet, and all teacher PDFs have been transferred to `Biology-Honors-V2`.
* **Dual Backwards-Compatibility in V2:** Even on the new domain ([`megaantony.github.io/high-school-biology-i-honors`](https://megaantony.github.io/high-school-biology-i-honors/)), redirect stubs at `Week-9-7/tests/` and `unit01-tests/` ensure that old bookmark paths work seamlessly.
* **Re-clonable anytime:** If you ever need a local copy of V1 in the future:
  ```bash
  git clone https://github.com/MegaAntony/biology-honors.git
  ```

---

## 🛠️ Step-by-Step Weekend Execution Instructions

When you are ready to perform the cleanup (e.g., Friday after school or over the weekend), run the following commands in Terminal:

### Option A: Move to macOS Trash (Recommended — Easily Recoverable)
Moving the directories to the macOS Trash allows you to empty them later while keeping them immediately out of the working folder:

```bash
# 1. Navigate to the Grade 9 directory
cd /Volumes/Backup/Antony/HighSchool/Grade9

# 2. Move the legacy scratch folder to macOS Trash
mv "Biology" ~/.Trash/

# 3. Move the legacy V1 clone to macOS Trash
mv "Biology-Honors" ~/.Trash/
```

---

### Option B: Direct Terminal Removal (Permanent)
If you want to free disk space immediately without using the Trash:

```bash
# 1. Remove the legacy unversioned scratch folder
rm -rf "/Volumes/Backup/Antony/HighSchool/Grade9/Biology"

# 2. Remove the local clone of V1
rm -rf "/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors"
```

---

## ✅ Post-Cleanup Verification Checklist

After removing the two legacy directories, verify that your new master workspace remains healthy:

1. **Verify Directory Structure:**
   ```bash
   ls -la /Volumes/Backup/Antony/HighSchool/Grade9/
   ```
   *Only `Biology-Honors-V2` should be present for Biology.*

2. **Verify Git Status in V2:**
   ```bash
   cd /Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors-V2
   git status
   ```
   *Should report: `On branch main, Your branch is up to date with 'origin/main', nothing to commit, working tree clean`.*

3. **Verify Both Live Sites in Browser:**
   * **New Master Portal:** [`https://megaantony.github.io/high-school-biology-i-honors/`](https://megaantony.github.io/high-school-biology-i-honors/) (200 OK)
   * **Legacy Bookmarks Portal:** [`https://megaantony.github.io/biology-honors/`](https://megaantony.github.io/biology-honors/) (200 OK)

4. **Verify Link Integrity:**
   ```bash
   python3 -c '
   import os, re, urllib.parse
   from pathlib import Path
   root = Path(".")
   html_md = list(root.glob("**/*.html")) + list(root.glob("**/*.md"))
   broken = []
   for f in html_md:
       if ".git" in f.parts: continue
       try: c = f.read_text(encoding="utf-8", errors="ignore")
       except: continue
       no_code = re.sub(r"```[\s\S]*?```", "", c)
       for raw in re.findall(r"href=[\"\x27]([^\s\"\x27>]+)[\"\x27]", no_code) + re.findall(r"\[[^\]]*\]\(([^)\s]+)\)", no_code):
           if raw.startswith(("http://", "https://", "mailto:", "javascript:", "#")): continue
           p = (f.parent / urllib.parse.unquote(raw.split("?")[0].split("#")[0])).resolve()
           if not p.exists(): broken.append((str(f.relative_to(root)), raw))
   print("✅ 0 broken links!" if not broken else f"❌ {len(broken)} broken")
   '
   ```

---

## 📞 Reference Links

* **New Master GitHub Repository:** [`MegaAntony/high-school-biology-i-honors`](https://github.com/MegaAntony/high-school-biology-i-honors)
* **New Production GitHub Pages:** [`https://megaantony.github.io/high-school-biology-i-honors/`](https://megaantony.github.io/high-school-biology-i-honors/)
* **Full Academic Year Ingestion Playbook:** [`ACADEMIC_YEAR_PLAN_AND_UNIT_PLAYBOOK.md`](ACADEMIC_YEAR_PLAN_AND_UNIT_PLAYBOOK.md)
* **Agent Operations & Standards Guide:** [`AGENT.md`](AGENT.md)
