# Getting started

Download the Windows executable from Releases. Verify SHA256 against the accompanying checksum file if desired. Double-click it and wait for the local browser interface. The standalone executable extracts its bundled runtime temporarily; keep the app running until you use Quit. No development environment or internet connection is needed after download.

Choose L2 n2 for the eight-cell coset8 reference, or L1 n2/n3 for one-cell degenerate references. Start with the supplied defaults. Couplings are nonnegative, dt is positive/dimensionless, and Steps is1..10000. Invalid/unsafe configurations are rejected before replacing valid state.

- Run new applies edits and prepares the declared reference.
- Pause stops actual computation after the current solver step.
- Resume continues the latest state, adding another active-setup step batch after completion.
- Reset applies edits and prepares the reference again.
- Cancel stops and retains the latest state.

Navigate up to512retained observations/states. Selecting earlier history pauses; Resume still continues the latest state. Save checkpoint exports the selected retained state. Plots/table values are computed source observables; no graviton or physical metric claim follows.

## Files

Save active setup exports configuration, not amplitudes. Open setup resets its reference paused. Save checkpoint contains all selected-state amplitudes; reset matching source/couplings before Open checkpoint to continue. Export results creates a manifested ZIP of observations/setup/gates/provenance; Open results is read-only. Export observations produces raw CSV; keep the ZIP for reliable provenance-aware reopening. Export SVG creates a standalone vector plot with raw metadata; view it in an SVG-capable browser.

File transfer uses browser uploads/downloads. Unique download names preserve older exports. Browser save-directory/collision prompts are controlled by the browser. Cancelling a picker leaves state unchanged. Legacy L2 result companions must be zipped together for import. Rejected malformed/changed/unsupported files preserve valid state.

## Refresh, closing and errors

Refresh reconnects within the browser session. Relaunch the executable to reopen the existing authorized service. Closing a tab does not stop computation. Use Quit to release backend/worker resources, then close the tab. Repeated launches reuse the existing app.

Windows startup diagnostics are written to `%LOCALAPPDATA%/Graviton/startup.log`. Missing-engine errors indicate a damaged executable/extraction; download the verified asset again. The app normally chooses an available local port. Do not terminate unrelated processes or disable system protections globally.

The Windows executable is unsigned. Its exact downloaded installation/reputation-warning experience needs fresh-host testing. Other Windows versions/browsers and native Mac/Linux packages are not accepted by the Windows checks.
