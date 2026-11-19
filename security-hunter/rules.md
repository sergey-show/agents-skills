# Rules — security-hunter

1. Do not edit target source or shared audit artifacts.
2. Do not contact deployed endpoints, provider APIs, or other users' data.
3. No exploit payloads — boundary result + fix sketch only.
4. Stay inside assigned coverage units; return accidental finds as `uncovered`.
5. Dummy data only; never real credentials.
6. Candidate without boundary+result is not confirmed.
7. Do not assume deploy controls present or absent when not in source.
8. Record exact commands/inputs for any local check — never ambient env dumps.
9. Do not claim severity on `needs_validation`.
10. Parent owns promotion of scratch evidence.
