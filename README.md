# Automated Sorting Cell — KUKA Robot + S7-1200 PLC
> An industrial pick-and-sort station: a KUKA arm sequenced by a Siemens S7-1200 PLC in Ladder, designed against recognised machine-safety standards.
`2025` · `KUKA` · `Siemens S7-1200` · `Ladder / TIA` · `ISO 13849-1` · `IEC 62061` · `Industrial automation`

![Automated Sorting Cell — KUKA Robot + S7-1200 PLC](docs/img/kuka-cell.svg)

## About

An industrial-automation project (with Chahin Dhaoui): an automated sorting cell built around a KUKA industrial robot that picks parts and sorts them by type, with a Siemens S7-1200 PLC as the cell controller and the two coordinated over their I/O handshake.

**The control lives in the PLC.** The sequencing — part present, robot request, pick, place, sort-by-destination, cycle complete — is written in Ladder on the S7-1200, which is the language a maintenance team on a real line actually reads and modifies. The robot executes motion; the PLC owns the logic, the interlocks and the cycle.

**Safety was a design input, not an afterthought.** The cell is specified against **ISO 13849-1** and **IEC 62061** — the standards that turn "add an emergency stop" into a quantified requirement on the safety function's performance level. Designing to them is the difference between a demo and something that could stand next to a person.

## Contents

```
docs/
```

## Notes

DOCUMENTATION ONLY - the deliverable was the cell design and its PLC ladder, written up as a report. The report PDFs are in `docs/`.

## Third-party work used here

Everything in this repository is my own work. It builds on the following, which are **not** mine and are used under their own licences:

- **KUKA KRL / KUKA.Sim** by KUKA — <https://kuka.com>
- **TIA Portal, S7-1200** by Siemens — <https://siemens.com>

## Author

Lassaad Mahmoudi — <assaadmahmoudi0@gmail.com>  
https://linkedin.com/in/mahmoudiassaad
