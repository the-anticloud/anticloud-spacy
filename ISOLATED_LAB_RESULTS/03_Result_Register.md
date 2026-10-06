# Result Register

**Project:** SPACY  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/explosion/spaCy @ c2dabfce56ad2991685ec85783cd59637a5d7b8f  
**Overlay:** anticloud/ (anticloud-ref v1.0.0)  
**Run:** 2026-10-06T09:27:30.223350+00:00  
**Aggregate:** PASS (16/16)

| Result | Pass Condition | Command (verbatim) | Observed | Status | SHA3-256 of evidence |
| --- | --- | --- | --- | --- | --- |
| 01_loc_files Code size and file count | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only 01_loc_files` | files=38 lines=8382 ceilings=20000 | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 02_licence Licence posture (A/B/C policy) | benchmark.ok == true and aggregate all_passed | `anticloud-ref licence-classify LICENSE && python tools/run_bench.py --only 02_licence` | project_licence={'LICENSE': 'A', 'reason': 'permissive licence text identified', 'spdx': 'mit'} | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 03_dependency_scan Dependency scan (hash-pinned lock) | benchmark.ok == true and aggregate all_passed | `anticloud-ref deps-verify requirements.lock` | pinned=6 hashed=6 problems=[] | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 04_sbom_cyclonedx SBOM (CycloneDX 1.5) | benchmark.ok == true and aggregate all_passed | `python -c "import json;d=json.load(open('sbom.cdx.json'));print(d['bomFormat'],d['specVersion'],len(d['components']))"` | CycloneDX 1.5 components=272 | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 05_git_health Git health | benchmark.ok == true and aggregate all_passed | `git status --porcelain && git log --oneline -1 && git fsck --no-progress` | head=92d76116dbdf4c9a73fee1968523a51de16cc051 commits=1 clean=True | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 06_owasp_llm_top10 OWASP Top 10 for LLM Applications | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only owasp` | 10/10 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 07_owasp_top10 OWASP Top 10 (2021) | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only owasp` | 9/9 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 08_soc2_type2 SOC 2 Type II readiness | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only soc2` | 9/9 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 09_nist_ai_rmf NIST AI Risk Management Framework | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only nist` | 8/8 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 10_nist_sp_800_53 NIST SP 800-53 Rev. 5 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only nist` | 12/12 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 11_nist_csf NIST Cybersecurity Framework 2.0 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only nist` | 8/8 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 12_fedramp FedRAMP Rev. 5 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only fedramp` | 10/10 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 13_pci_dss PCI DSS v4.0.1 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only pci` | 11/11 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 14_iso_27001 ISO/IEC 27001:2022 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only iso` | 9/9 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 15_mitre_attack MITRE ATT&CK v16 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only mitre` | 12/12 controls evidenced (100.0%) | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |
| 16_ml_trl ML Technology Readiness Level 8 | benchmark.ok == true and aggregate all_passed | `python tools/run_bench.py --only 16 && cat docs/18_TRL_JUSTIFICATION/TRL.md` | trl=8 satisfied=8/8 missing=[] | PASS | `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee` |

Aggregate row: all 16 checks AND-ed. Evidence file: `ISOLATED_LAB_RESULTS/04_Evidence/16_checks_report.json` (SHA3-256 `14b7a539c453aae6a65762be8e9a2dcbc3d0f112806e87b9697dc17ce64b34ee`).

> Hash correction 2026-10-06: BENCH.json was modified by the contamination scrub (credential strip / upstream-head fix) after this register was written. Current BENCH.json sha3-256: 4c9976c60c22443233ac79c47cb147372eb45731d7d4e1eaafbda603f225b2ab. Original recorded hashes above are the pre-scrub snapshots and are kept as audit trail.
